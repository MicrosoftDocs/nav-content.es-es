---
title: "Introducción de códigos CCC"
description: "El Código Cuenta Cliente (CCC) es un código de identificación de cuentas bancarias único. Los siguientes campos de componentes componen la estructura de código CCC de 20 dígitos (España) o 21 dígitos (Portugal)."
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
ms.openlocfilehash: 1e534da91f34caa543d62f11ecba660c62b30556
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enter-ccc-codes"></a><span data-ttu-id="7d084-104">Introducción de códigos CCC</span><span class="sxs-lookup"><span data-stu-id="7d084-104">How to: Enter CCC Codes</span></span>
<span data-ttu-id="7d084-105">El Código Cuenta Cliente (CCC) es un código de identificación de cuentas bancarias único.</span><span class="sxs-lookup"><span data-stu-id="7d084-105">Código Cuenta Cliente (CCC) is a unique bank account identification code.</span></span> <span data-ttu-id="7d084-106">Los siguientes campos de componentes componen la estructura de código CCC de 20 dígitos (España) o 21 dígitos (Portugal).</span><span class="sxs-lookup"><span data-stu-id="7d084-106">The following component fields make up the 20-digit (Spain) or 21-digit (Portugal) bank CCC code structure.</span></span>  
  
 <span data-ttu-id="7d084-107">Si modifica la estructura del código CCC, el campo **Nº CCC**</span><span class="sxs-lookup"><span data-stu-id="7d084-107">If you change the CCC code structure, the **CCC No.**</span></span> <span data-ttu-id="7d084-108">se actualiza automáticamente.</span><span class="sxs-lookup"><span data-stu-id="7d084-108">field updates automatically.</span></span> <span data-ttu-id="7d084-109">De igual forma, si modifica el campo **Nº CCC**</span><span class="sxs-lookup"><span data-stu-id="7d084-109">Similarly, if you change the **CCC No.**</span></span> <span data-ttu-id="7d084-110">la estructura del código CCC se actualiza automáticamente.</span><span class="sxs-lookup"><span data-stu-id="7d084-110">field, the CCC code structure updates automatically.</span></span>  
  
### <a name="to-enter-ccc-codes"></a><span data-ttu-id="7d084-111">Para introducir códigos CCC</span><span class="sxs-lookup"><span data-stu-id="7d084-111">To enter CCC codes</span></span>  
  
1.  <span data-ttu-id="7d084-112">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Información de la empresa** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="7d084-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="7d084-113">Rellene los campos de la ficha desplegable **Pagos**, tal como se describe en la tabla siguiente</span><span class="sxs-lookup"><span data-stu-id="7d084-113">On the **Payments** FastTab, fill in the fields as described in the following table</span></span>  
  
    |<span data-ttu-id="7d084-114">Campo</span><span class="sxs-lookup"><span data-stu-id="7d084-114">Field</span></span>|<span data-ttu-id="7d084-115">Description</span><span class="sxs-lookup"><span data-stu-id="7d084-115">Description</span></span>|  
    |---------------------------------|--------------|---------------------------------------|  
    |<span data-ttu-id="7d084-116">**CCC Cód. banco**</span><span class="sxs-lookup"><span data-stu-id="7d084-116">**CCC Bank No.**</span></span>|<span data-ttu-id="7d084-117">1-4</span><span class="sxs-lookup"><span data-stu-id="7d084-117">1-4</span></span>|<span data-ttu-id="7d084-118">Identifica el banco en el que se ha abierto la cuenta.</span><span class="sxs-lookup"><span data-stu-id="7d084-118">Identifies the bank where the account has been opened.</span></span>|  
    |<span data-ttu-id="7d084-119">**CCC Cód. oficina**</span><span class="sxs-lookup"><span data-stu-id="7d084-119">**CCC Bank Branch No.**</span></span>|<span data-ttu-id="7d084-120">5-8</span><span class="sxs-lookup"><span data-stu-id="7d084-120">5-8</span></span>|<span data-ttu-id="7d084-121">Identifica el código de la oficina.</span><span class="sxs-lookup"><span data-stu-id="7d084-121">Identifies the branch code.</span></span> <span data-ttu-id="7d084-122">Si el banco no utiliza esta referencia, pueden ser ceros.</span><span class="sxs-lookup"><span data-stu-id="7d084-122">If the bank does not use this reference, these can be zeros.</span></span>|  
    |<span data-ttu-id="7d084-123">**CCC Dígito control**</span><span class="sxs-lookup"><span data-stu-id="7d084-123">**CCC Control Digits**</span></span>|<span data-ttu-id="7d084-124">9-10</span><span class="sxs-lookup"><span data-stu-id="7d084-124">9-10</span></span>|<span data-ttu-id="7d084-125">Identifica los dígitos de control.</span><span class="sxs-lookup"><span data-stu-id="7d084-125">Identifies the control digits.</span></span>|  
    |<span data-ttu-id="7d084-126">**CCC Nº cuenta**</span><span class="sxs-lookup"><span data-stu-id="7d084-126">**CCC Bank Account No.**</span></span>|<span data-ttu-id="7d084-127">11-20 (España)</span><span class="sxs-lookup"><span data-stu-id="7d084-127">11-20 (Spain)</span></span><br /><br /> <span data-ttu-id="7d084-128">11-21 (Portugal)</span><span class="sxs-lookup"><span data-stu-id="7d084-128">11-21 (Portugal)</span></span>|<span data-ttu-id="7d084-129">Identifica el número de cuenta, que se puede ajustar con ceros a la izquierda.</span><span class="sxs-lookup"><span data-stu-id="7d084-129">Identifies the account number, which may be adjusted with preceding zeros.</span></span>|  
  
## <a name="see-also"></a><span data-ttu-id="7d084-130">Consulte también</span><span class="sxs-lookup"><span data-stu-id="7d084-130">See Also</span></span>  
 [<span data-ttu-id="7d084-131">Funcionalidad local para España</span><span class="sxs-lookup"><span data-stu-id="7d084-131">Spain Local Functionality</span></span>](spain-local-functionality.md)
