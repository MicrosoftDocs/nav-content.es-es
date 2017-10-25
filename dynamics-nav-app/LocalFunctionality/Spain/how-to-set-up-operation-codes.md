---
title: "Configuración de códigos de operación"
description: "Puede añadir tantos códigos de operación como desee a la tabla. Sin embargo, los códigos C, D e I ya existe en Microsoft Dynamics NAV. Por ejemplo, los abonos siempre tienen el código de operación D. No puede configurar estos valores en la tabla porque son códigos creados por el sistema. Si intenta agregarlos, Microsoft Dynamics NAV devolverá un error."
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
ms.openlocfilehash: ee8d48e7ab1935afb4bbe65a859f4fb9a3672473
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-operation-codes"></a><span data-ttu-id="6953d-106">Configuración de códigos de operación</span><span class="sxs-lookup"><span data-stu-id="6953d-106">How to: Set Up Operation Codes</span></span>
<span data-ttu-id="6953d-107">Puede añadir tantos códigos de operación como desee a la tabla.</span><span class="sxs-lookup"><span data-stu-id="6953d-107">You can add as many operation codes as you want to the table.</span></span> <span data-ttu-id="6953d-108">Sin embargo, los códigos C, D e I ya existe en Microsoft Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="6953d-108">However, the operation codes C, D, and I already exist in Microsoft Dynamics NAV.</span></span> <span data-ttu-id="6953d-109">Por ejemplo, los abonos siempre tienen el código de operación D. No puede configurar estos valores en la tabla porque son códigos creados por el sistema.</span><span class="sxs-lookup"><span data-stu-id="6953d-109">For example, Credit Memos always have the operation code D. You cannot set up these values in the table because they are system-created codes.</span></span> <span data-ttu-id="6953d-110">Si intenta agregarlos, Microsoft Dynamics NAV devolverá un error.</span><span class="sxs-lookup"><span data-stu-id="6953d-110">If you try to add them, Microsoft Dynamics NAV will return an error.</span></span>  
  
### <a name="to-set-up-operation-codes"></a><span data-ttu-id="6953d-111">Para configurar códigos de operación</span><span class="sxs-lookup"><span data-stu-id="6953d-111">To set up operation codes</span></span>  
  
1.  <span data-ttu-id="6953d-112">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Códigos de operación** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="6953d-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Operation Codes**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="6953d-113">En la ventana **Códigos de operación**, rellene los campos tal como se describe en la tabla siguiente</span><span class="sxs-lookup"><span data-stu-id="6953d-113">In the **Operation Codes** window, fill in the fields as described in the following table</span></span>  
  
    |<span data-ttu-id="6953d-114">Campo</span><span class="sxs-lookup"><span data-stu-id="6953d-114">Field</span></span>|<span data-ttu-id="6953d-115">Description</span><span class="sxs-lookup"><span data-stu-id="6953d-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="6953d-116">**Código**</span><span class="sxs-lookup"><span data-stu-id="6953d-116">**Code**</span></span>|<span data-ttu-id="6953d-117">Introduzca un código de operación.</span><span class="sxs-lookup"><span data-stu-id="6953d-117">Enter an operation code.</span></span> <span data-ttu-id="6953d-118">Puede introducir un letra o número.</span><span class="sxs-lookup"><span data-stu-id="6953d-118">You can only enter one letter or number.</span></span><br /><br /> <span data-ttu-id="6953d-119">Los códigos válidos son números del 1 al 8 y letras de la A a la Z.</span><span class="sxs-lookup"><span data-stu-id="6953d-119">Valid codes are numbers 1 – 8, and letters A – Z.</span></span><br /><br /> <span data-ttu-id="6953d-120">Para enviar un informe bajo el régimen de CAC, debe asegurarse de que el código Z, que se requiere para este tipo de transacciones, se encuentre en la lista de códigos de operación.</span><span class="sxs-lookup"><span data-stu-id="6953d-120">To submit a report under the CAC regimen, you must make certain that the code Z, which is required for these types of transactions, is in the list of operation codes.</span></span>|  
    |<span data-ttu-id="6953d-121">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="6953d-121">**Description**</span></span>|<span data-ttu-id="6953d-122">Escriba una descripción para el código de operación.</span><span class="sxs-lookup"><span data-stu-id="6953d-122">Enter a description for the operation code.</span></span> <span data-ttu-id="6953d-123">Puede introducir un máximo de 30 caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="6953d-123">You can enter a maximum of 30 letters and numbers.</span></span>|  
  
### <a name="to-link-operation-codes-to-general-product-posting-groups"></a><span data-ttu-id="6953d-124">Para vincular códigos de operación a grupos de publicación de productos en general</span><span class="sxs-lookup"><span data-stu-id="6953d-124">To link operation codes to general product posting groups</span></span>  
  
1.  <span data-ttu-id="6953d-125">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos contables** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="6953d-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posting Groups**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="6953d-126">Elija **Grupos contables de producto general**.</span><span class="sxs-lookup"><span data-stu-id="6953d-126">Choose **General Product Posting Groups**.</span></span>  
  
3.  <span data-ttu-id="6953d-127">En la ventana Grupos de publicación de productos generales, vincule cada código de operación a un grupo de publicación de productos general.</span><span class="sxs-lookup"><span data-stu-id="6953d-127">In the General Product Posting Groups window, link each operation code to a general product posting group.</span></span>  
  
    |<span data-ttu-id="6953d-128">Campo</span><span class="sxs-lookup"><span data-stu-id="6953d-128">Field</span></span>|<span data-ttu-id="6953d-129">Description</span><span class="sxs-lookup"><span data-stu-id="6953d-129">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="6953d-130">Código</span><span class="sxs-lookup"><span data-stu-id="6953d-130">Code</span></span>|<span data-ttu-id="6953d-131">Introduzca un código para crear un nuevo grupo contable de producto general.</span><span class="sxs-lookup"><span data-stu-id="6953d-131">Enter a code to create a new general product posting group.</span></span>|  
    |<span data-ttu-id="6953d-132">Description</span><span class="sxs-lookup"><span data-stu-id="6953d-132">Description</span></span>|<span data-ttu-id="6953d-133">Introduzca una descripción del grupo contable de producto general</span><span class="sxs-lookup"><span data-stu-id="6953d-133">Enter a description for the general product posting group</span></span>|  
    |<span data-ttu-id="6953d-134">Grupo reg. IVA prod. genér.</span><span class="sxs-lookup"><span data-stu-id="6953d-134">Def. VAT Prod. Posting Group</span></span>|<span data-ttu-id="6953d-135">Seleccione un porcentaje de IVA para vincularlo al grupo de publicación de producto general.</span><span class="sxs-lookup"><span data-stu-id="6953d-135">Select a VAT percentage to link it to the general product posting group.</span></span>|  
    |<span data-ttu-id="6953d-136">Código operación</span><span class="sxs-lookup"><span data-stu-id="6953d-136">Operation Code</span></span>|<span data-ttu-id="6953d-137">Seleccione una operación apropiada para vincularla a un grupo contable de producto general.</span><span class="sxs-lookup"><span data-stu-id="6953d-137">Select an appropriate operation code to link it to the general product posting group.</span></span> <span data-ttu-id="6953d-138">Puede asignar el mismo código de operación a distintos grupos contables.</span><span class="sxs-lookup"><span data-stu-id="6953d-138">You can assigne the same operation code to different posting groups.</span></span> <span data-ttu-id="6953d-139">**Nota:** Es importante vincular el código de operación al grupo de registro de IVA de producto correcto.</span><span class="sxs-lookup"><span data-stu-id="6953d-139">**Note:**  It is important to link the operation code to the correct VAT product posting group.</span></span> <span data-ttu-id="6953d-140">El informe del modelo 340 usa la configuración para crear declaraciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="6953d-140">The Make 340 Declaration report uses the setup to create trade declarations.</span></span>|  
  
 <span data-ttu-id="6953d-141">Cuando agrega un código de operación al grupo de publicación de producto general, esa asociación se aplica a su vez a los artículos que tienen ese grupo.</span><span class="sxs-lookup"><span data-stu-id="6953d-141">When you add an operation code to the general product posting group, that association is in turn applied to the items that have that general product posting group.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="6953d-142">Consulte también</span><span class="sxs-lookup"><span data-stu-id="6953d-142">See Also</span></span>  
 [<span data-ttu-id="6953d-143">Creación del informe 340</span><span class="sxs-lookup"><span data-stu-id="6953d-143">How to: Create Report 340</span></span>](how-to-create-report-340.md)
