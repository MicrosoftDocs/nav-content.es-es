---
title: "Detalles de diseño: estructura de motor de registro"
description: "La interfaz de registro y otras funciones en la unidad de código 12 utilizan funciones de motor de registro para preparar e insertar movimientos de contabilidad y registros de movimientos de IVA. El motor de registro también es responsable de la creación del registro de contabilidad."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2a0c90fde23b708c3de8365f7211e66bee615cb1
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-engine-structure"></a><span data-ttu-id="00c8f-104">Detalles de diseño: estructura de motor de registro</span><span class="sxs-lookup"><span data-stu-id="00c8f-104">Design Details: Posting Engine Structure</span></span>
<span data-ttu-id="00c8f-105">La interfaz de registro y otras funciones en la unidad de código 12 utilizan funciones de motor de registro para preparar e insertar movimientos de contabilidad y registros de movimientos de IVA.</span><span class="sxs-lookup"><span data-stu-id="00c8f-105">Posting interface and some other functions in codeunit 12 use posting engine functions to prepare and insert general ledger entry and VAT entry records.</span></span> <span data-ttu-id="00c8f-106">El motor de registro también es responsable de la creación del registro de contabilidad.</span><span class="sxs-lookup"><span data-stu-id="00c8f-106">The posting engine is also responsible for general ledger register creation.</span></span>  
  
 <span data-ttu-id="00c8f-107">Las funciones en la tabla siguiente proporcionan un marco estándar para diseñar procedimientos de registro (como Code, CustPostApplyCustledgEntry, VendPostApplyVendLedgEntry, UnapplyCustLedgEntry, UnapplyVendLedgEntry y Reverse) y acceso exclusivo a la tabla 17, Mov. C/G.</span><span class="sxs-lookup"><span data-stu-id="00c8f-107">The functions in the following table provide a standard framework for designing posting procedures (such as Code, CustPostApplyCustledgEntry, VendPostApplyVendLedgEntry, UnapplyCustLedgEntry, UnapplyVendLedgEntry, and Reverse) and exclusive access to table 17, G/L Entry.</span></span>  
  
|<span data-ttu-id="00c8f-108">Routine</span><span class="sxs-lookup"><span data-stu-id="00c8f-108">Routine</span></span>|<span data-ttu-id="00c8f-109">Description</span><span class="sxs-lookup"><span data-stu-id="00c8f-109">Description</span></span>|  
|-------------|---------------------------------------|  
|<span data-ttu-id="00c8f-110">StartPosting</span><span class="sxs-lookup"><span data-stu-id="00c8f-110">StartPosting</span></span>|<span data-ttu-id="00c8f-111">Inicializa el búfer de registro TempGLEntryBuf, bloquea las tablas de movimientos de contabilidad y de IVA e inicializa el periodo contable, el registro de contabilidad y el tipo de cambio.</span><span class="sxs-lookup"><span data-stu-id="00c8f-111">Initializes posting buffer TempGLEntryBuf, locks G/L Entry and VAT Entry tables, and initializes Accounting Period, G/L Register, and Exchange Rate.</span></span> <span data-ttu-id="00c8f-112">Si se le llama solo una vez, NextEntryNo es 0.</span><span class="sxs-lookup"><span data-stu-id="00c8f-112">Should be called only once, then NextEntryNo is 0.</span></span>|  
|<span data-ttu-id="00c8f-113">ContinuePosting</span><span class="sxs-lookup"><span data-stu-id="00c8f-113">ContinuePosting</span></span>|<span data-ttu-id="00c8f-114">Comprueba y registra el IVA no realizado para el incremento NextTransactionNo de la transacción anterior y prepara el registro de la línea siguiente.</span><span class="sxs-lookup"><span data-stu-id="00c8f-114">Checks and posts unrealized VAT for previous transaction increment NextTransactionNo and prepares post of next line.</span></span>|  
|<span data-ttu-id="00c8f-115">FinishPosting</span><span class="sxs-lookup"><span data-stu-id="00c8f-115">FinishPosting</span></span>|<span data-ttu-id="00c8f-116">Finaliza el registro insertando los movimientos de contabilidad desde el búfer temporal a la tabla de la base de datos.</span><span class="sxs-lookup"><span data-stu-id="00c8f-116">Completes posting by inserting G/L entries from temporary buffer into database table.</span></span> <span data-ttu-id="00c8f-117">Se utiliza siempre con StartPosting.</span><span class="sxs-lookup"><span data-stu-id="00c8f-117">Always used together with StartPosting.</span></span> <span data-ttu-id="00c8f-118">Comprueba la presencia de inconsistencias.</span><span class="sxs-lookup"><span data-stu-id="00c8f-118">Checks for inconsistencies.</span></span>|  
|<span data-ttu-id="00c8f-119">InitGLEntry</span><span class="sxs-lookup"><span data-stu-id="00c8f-119">InitGLEntry</span></span>|<span data-ttu-id="00c8f-120">Se utiliza para inicializar un nuevo movimiento de contabilidad para la línea de diario general.</span><span class="sxs-lookup"><span data-stu-id="00c8f-120">Used to initialize new G/L entry for Gen. Jnl Line.</span></span> <span data-ttu-id="00c8f-121">Devuelve GLEntry como parámetro.</span><span class="sxs-lookup"><span data-stu-id="00c8f-121">Returns GLEntry as parameter.</span></span>|  
|<span data-ttu-id="00c8f-122">InitGLEntryVAT</span><span class="sxs-lookup"><span data-stu-id="00c8f-122">InitGLEntryVAT</span></span>|<span data-ttu-id="00c8f-123">Igual que InitGLEntry, pero también asigna Cta. contrapartida y SummarizeVAT.</span><span class="sxs-lookup"><span data-stu-id="00c8f-123">Same as InitGLEntry, but also assigns Bal. Account No. and SummarizeVAT.</span></span>|  
|<span data-ttu-id="00c8f-124">InitGLEntryVATCopy</span><span class="sxs-lookup"><span data-stu-id="00c8f-124">InitGLEntryVATCopy</span></span>|<span data-ttu-id="00c8f-125">Similar a InitGLEntryVAT, pero también copia datos de grupos de registro desde movimientos de IVA antes de SummarizeVAT.</span><span class="sxs-lookup"><span data-stu-id="00c8f-125">Similar to InitGLEntryVAT, but also copies posting groups data from VAT Entry before SummarizeVAT.</span></span>|  
|<span data-ttu-id="00c8f-126">InsertGLEntry</span><span class="sxs-lookup"><span data-stu-id="00c8f-126">InsertGLEntry</span></span>|<span data-ttu-id="00c8f-127">La única función que inserta el movimiento de contabilidad general en la tabla global TempGLEntryBuf.</span><span class="sxs-lookup"><span data-stu-id="00c8f-127">The only function that inserts G/L entry into global TempGLEntryBuf table.</span></span> <span data-ttu-id="00c8f-128">Utilice siempre esta función para insertar.</span><span class="sxs-lookup"><span data-stu-id="00c8f-128">Always use this function for insert.</span></span>|  
|<span data-ttu-id="00c8f-129">CreateGLEntry</span><span class="sxs-lookup"><span data-stu-id="00c8f-129">CreateGLEntry</span></span>|<span data-ttu-id="00c8f-130">Lleva a cabo una acción InitGLEntry, asigna un importe adicional de divisa y realiza una acción InsertGLEntry.</span><span class="sxs-lookup"><span data-stu-id="00c8f-130">Performs an InitGLEntry, assigns Additional Currency Amount, and then performs InsertGLEntry.</span></span> <span data-ttu-id="00c8f-131">Reemplaza varias líneas de código con una sola llamada a función.</span><span class="sxs-lookup"><span data-stu-id="00c8f-131">Replaces several lines of code with a single function call.</span></span>|  
|<span data-ttu-id="00c8f-132">CreateGLEntryBalAcc</span><span class="sxs-lookup"><span data-stu-id="00c8f-132">CreateGLEntryBalAcc</span></span>|<span data-ttu-id="00c8f-133">Igual que CreateGLEntry, pero también asigna Tipo contrapartida y Cta. contrapartida.</span><span class="sxs-lookup"><span data-stu-id="00c8f-133">Same as CreateGLEntry, but also assigns Bal. Account Type and Bal. Account No.</span></span>|  
|<span data-ttu-id="00c8f-134">CreateGLEntryVAT</span><span class="sxs-lookup"><span data-stu-id="00c8f-134">CreateGLEntryVAT</span></span>|<span data-ttu-id="00c8f-135">Igual que CreateGLEntry, pero con procesamiento adicional para grupos de registro y guardado en búfer temporal de IVA:</span><span class="sxs-lookup"><span data-stu-id="00c8f-135">Same as CreateGLEntry, but with additional processing for posting groups and saving to temporary VAT buffer:</span></span><br /><br /> `GLEntry.CopyPostingGroupsFromDtldCVBuf(DtldCVLedgEntryBuf,GenJnlLine."Gen. Posting Type");`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|<span data-ttu-id="00c8f-136">CreateGLEntryVATCollectAdj</span><span class="sxs-lookup"><span data-stu-id="00c8f-136">CreateGLEntryVATCollectAdj</span></span>|<span data-ttu-id="00c8f-137">Igual que CreateGLEntry, pero con recopilación adicional de ajustes y guardado en búfer temporal de IVA:</span><span class="sxs-lookup"><span data-stu-id="00c8f-137">Same as CreateGLEntry, but with additional collection of adjustments and saving to temporary VAT buffer:</span></span><br /><br /> `CollectAdjustment(AdjAmount,GLEntry.Amount,GLEntry."Additional-Currency Amount",OriginalDateSet);`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|<span data-ttu-id="00c8f-138">CreateGLEntryFromVATEntry</span><span class="sxs-lookup"><span data-stu-id="00c8f-138">CreateGLEntryFromVATEntry</span></span>|<span data-ttu-id="00c8f-139">Igual que CreateGLEntry, pero también copia grupos de registro desde movimientos de IVA.</span><span class="sxs-lookup"><span data-stu-id="00c8f-139">Same as CreateGLEntry, but also copies posting groups from VAT entry.</span></span>|  
  
## <a name="see-also"></a><span data-ttu-id="00c8f-140">Consulte también</span><span class="sxs-lookup"><span data-stu-id="00c8f-140">See Also</span></span>  
 [<span data-ttu-id="00c8f-141">Detalles de diseño: estructura de interfaz de registro</span><span class="sxs-lookup"><span data-stu-id="00c8f-141">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)