---
title: "Transferencia automática y movimientos combinados"
description: "En contabilidad de costes, puede transferir los movimientos de contabilidad a un tipo de coste mediante un registro combinado. Puede especificar si un tipo de coste recibe las movimientos agrupados en el campo **Combinar movimientos** en la definición del tipo de coste. La siguiente tabla describe las distintas opciones."
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
ms.openlocfilehash: 638fc123d4113695d70102a94b9fce0bff6b43fa
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="f8dc3-105">Transferencia automática y movimientos combinados</span><span class="sxs-lookup"><span data-stu-id="f8dc3-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="f8dc3-106">En contabilidad de costes, puede transferir los movimientos de contabilidad a un tipo de coste mediante un registro combinado.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="f8dc3-107">Puede especificar si un tipo de coste recibe las movimientos agrupados en el campo **Combinar movimientos** en la definición del tipo de coste.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="f8dc3-108">La siguiente tabla describe las distintas opciones.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="f8dc3-109">Combinar movimientos</span><span class="sxs-lookup"><span data-stu-id="f8dc3-109">Combine entries</span></span>|<span data-ttu-id="f8dc3-110">Descripción</span><span class="sxs-lookup"><span data-stu-id="f8dc3-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="f8dc3-111">Ninguno</span><span class="sxs-lookup"><span data-stu-id="f8dc3-111">None</span></span>|<span data-ttu-id="f8dc3-112">Cada movimiento de contabilidad se transfiere individualmente al tipo de coste correspondiente.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="f8dc3-113">Día</span><span class="sxs-lookup"><span data-stu-id="f8dc3-113">Day</span></span>|<span data-ttu-id="f8dc3-114">Los movimientos de contabilidad que tienen la misma fecha de registro se transfieren como un solo movimiento al tipo de coste correspondiente.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="f8dc3-115">Mes</span><span class="sxs-lookup"><span data-stu-id="f8dc3-115">Month</span></span>|<span data-ttu-id="f8dc3-116">Todos los movimientos de contabilidad general que tienen el mismo mes de calendario se transfieren como un solo movimiento al tipo de coste correspondiente.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="f8dc3-117">Si ha seleccionado la casilla **Transf. autom. desde C/G** en la ventana **Configuración contabilidad costes**, [!INCLUDE[d365fin](includes/d365fin_md.md)] actualiza la contabilidad de costes después de cada registro en la contabilidad.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="f8dc3-118">Ya no se pueden realizar movimientos combinados.</span><span class="sxs-lookup"><span data-stu-id="f8dc3-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f8dc3-119">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f8dc3-119">See Also</span></span>  
 <span data-ttu-id="f8dc3-120">[Procedimiento: transferencia de movimientos de contabilidad a los movimientos de coste](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f8dc3-120">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="f8dc3-121">[Criterios para la transferencia de movimientos de contabilidad a movimientos de coste](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f8dc3-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="f8dc3-122">[Resultados de la transferencia](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="f8dc3-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="f8dc3-123">Transferencia y registro de movimientos de coste</span><span class="sxs-lookup"><span data-stu-id="f8dc3-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="f8dc3-124">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f8dc3-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
