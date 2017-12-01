---
title: "Configuración de códigos de operación"
description: "Puede añadir tantos códigos de operación como desee a la tabla. Sin embargo, los códigos C, D e I ya existen en [!INCLUDE[navnow](../../includes/navnow_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: abeb802b3e478b04a4b50915121fd7d17d355633
ms.contentlocale: es-es
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-operation-codes"></a><span data-ttu-id="bdc3f-104">Configuración de códigos de operación</span><span class="sxs-lookup"><span data-stu-id="bdc3f-104">How to: Set Up Operation Codes</span></span>
<span data-ttu-id="bdc3f-105">Puede añadir tantos códigos de operación como desee a la tabla.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-105">You can add as many operation codes as you want to the table.</span></span> <span data-ttu-id="bdc3f-106">Sin embargo, los códigos C, D e I ya existe en [!INCLUDE[navnow](../../includes/navnow_md.md)].</span><span class="sxs-lookup"><span data-stu-id="bdc3f-106">However, the operation codes C, D, and I already exist in [!INCLUDE[navnow](../../includes/navnow_md.md)].</span></span> <span data-ttu-id="bdc3f-107">Por ejemplo, los abonos siempre tienen el código de operación D. No puede configurar estos valores en la tabla porque son códigos creados por el sistema.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-107">For example, Credit Memos always have the operation code D. You cannot set up these values in the table because they are system-created codes.</span></span> <span data-ttu-id="bdc3f-108">Si intenta agregarlos, [!INCLUDE[navnow](../../includes/navnow_md.md)] devolverá un error.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-108">If you try to add them, [!INCLUDE[navnow](../../includes/navnow_md.md)] will return an error.</span></span>  

## <a name="to-set-up-operation-codes"></a><span data-ttu-id="bdc3f-109">Para configurar códigos de operación</span><span class="sxs-lookup"><span data-stu-id="bdc3f-109">To set up operation codes</span></span>  

1.  <span data-ttu-id="bdc3f-110">Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Códigos de operación** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Operation Codes**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bdc3f-111">En la ventana **Códigos de operación**, rellene los campos tal como se describe en la tabla siguiente</span><span class="sxs-lookup"><span data-stu-id="bdc3f-111">In the **Operation Codes** window, fill in the fields as described in the following table</span></span>  

    |<span data-ttu-id="bdc3f-112">Campo</span><span class="sxs-lookup"><span data-stu-id="bdc3f-112">Field</span></span>|<span data-ttu-id="bdc3f-113">Description</span><span class="sxs-lookup"><span data-stu-id="bdc3f-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="bdc3f-114">**Código**</span><span class="sxs-lookup"><span data-stu-id="bdc3f-114">**Code**</span></span>|<span data-ttu-id="bdc3f-115">Introduzca un código de operación.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-115">Enter an operation code.</span></span> <span data-ttu-id="bdc3f-116">Puede introducir un letra o número.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-116">You can only enter one letter or number.</span></span><br /><br /> <span data-ttu-id="bdc3f-117">Los códigos válidos son números del 1 al 8 y letras de la A a la Z.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-117">Valid codes are numbers 1 – 8, and letters A – Z.</span></span><br /><br /> <span data-ttu-id="bdc3f-118">Para enviar un informe bajo el régimen de CAC, debe asegurarse de que el código Z, que se requiere para este tipo de transacciones, se encuentre en la lista de códigos de operación.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-118">To submit a report under the CAC regimen, you must make certain that the code Z, which is required for these types of transactions, is in the list of operation codes.</span></span>|  
    |<span data-ttu-id="bdc3f-119">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="bdc3f-119">**Description**</span></span>|<span data-ttu-id="bdc3f-120">Escriba una descripción para el código de operación.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-120">Enter a description for the operation code.</span></span> <span data-ttu-id="bdc3f-121">Puede introducir un máximo de 30 caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-121">You can enter a maximum of 30 letters and numbers.</span></span>|  

## <a name="to-link-operation-codes-to-general-product-posting-groups"></a><span data-ttu-id="bdc3f-122">Para vincular códigos de operación a grupos de publicación de productos en general</span><span class="sxs-lookup"><span data-stu-id="bdc3f-122">To link operation codes to general product posting groups</span></span>  

1.  <span data-ttu-id="bdc3f-123">Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos contables** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-123">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posting Groups**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bdc3f-124">Elija la acción **Grupos contables de producto general**.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-124">Choose the **General Product Posting Groups** action.</span></span>  
3.  <span data-ttu-id="bdc3f-125">En la ventana **Grupos de publicación de productos generales**, vincule cada código de operación a un grupo de publicación de productos general.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-125">In the **General Product Posting Groups** window, link each operation code to a general product posting group.</span></span>  

    |<span data-ttu-id="bdc3f-126">Campo</span><span class="sxs-lookup"><span data-stu-id="bdc3f-126">Field</span></span>|<span data-ttu-id="bdc3f-127">Description</span><span class="sxs-lookup"><span data-stu-id="bdc3f-127">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="bdc3f-128">Código</span><span class="sxs-lookup"><span data-stu-id="bdc3f-128">Code</span></span>|<span data-ttu-id="bdc3f-129">Introduzca un código para crear un nuevo grupo contable de producto general.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-129">Enter a code to create a new general product posting group.</span></span>|  
    |<span data-ttu-id="bdc3f-130">Description</span><span class="sxs-lookup"><span data-stu-id="bdc3f-130">Description</span></span>|<span data-ttu-id="bdc3f-131">Introduzca una descripción del grupo contable de producto general</span><span class="sxs-lookup"><span data-stu-id="bdc3f-131">Enter a description for the general product posting group</span></span>|  
    |<span data-ttu-id="bdc3f-132">Grupo reg. IVA prod. genér.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-132">Def. VAT Prod. Posting Group</span></span>|<span data-ttu-id="bdc3f-133">Seleccione un porcentaje de IVA para vincularlo al grupo de publicación de producto general.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-133">Select a VAT percentage to link it to the general product posting group.</span></span>|  
    |<span data-ttu-id="bdc3f-134">Código operación</span><span class="sxs-lookup"><span data-stu-id="bdc3f-134">Operation Code</span></span>|<span data-ttu-id="bdc3f-135">Seleccione una operación apropiada para vincularla a un grupo contable de producto general.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-135">Select an appropriate operation code to link it to the general product posting group.</span></span> <span data-ttu-id="bdc3f-136">Puede asignar el mismo código de operación a distintos grupos contables.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-136">You can assigne the same operation code to different posting groups.</span></span> <span data-ttu-id="bdc3f-137">**Nota:** Es importante vincular el código de operación al grupo de registro de IVA de producto correcto.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-137">**Note:**  It is important to link the operation code to the correct VAT product posting group.</span></span> <span data-ttu-id="bdc3f-138">El informe del modelo 340 usa la configuración para crear declaraciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-138">The Make 340 Declaration report uses the setup to create trade declarations.</span></span>|  

<span data-ttu-id="bdc3f-139">Cuando agrega un código de operación al grupo de publicación de producto general, esa asociación se aplica a su vez a los artículos que tienen ese grupo.</span><span class="sxs-lookup"><span data-stu-id="bdc3f-139">When you add an operation code to the general product posting group, that association is in turn applied to the items that have that general product posting group.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bdc3f-140">Consulte también</span><span class="sxs-lookup"><span data-stu-id="bdc3f-140">See Also</span></span>  
 [<span data-ttu-id="bdc3f-141">Creación del informe 340</span><span class="sxs-lookup"><span data-stu-id="bdc3f-141">How to: Create Report 340</span></span>](how-to-create-report-340.md)

