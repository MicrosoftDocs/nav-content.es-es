---
title: Asignar las ubicaciones predefinidas a los productos
description: "Si utiliza ubicaciones en un almacén, la asignación de ubicaciones genéricas a sus productos puede facilitar el proceso de envío, recepción y movimiento de sus productos. Cuando se asigna una ubicación genérica a un producto, se sugiere esta ubicación cada vez que se inicia una transacción de este producto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c046cb3631cd690ba4bf4a1f1147f6e03d7cec9a
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-assign-default-bins-to-items"></a><span data-ttu-id="9dc24-104">Procedimiento: asigne las ubicaciones predefinidas a los productos</span><span class="sxs-lookup"><span data-stu-id="9dc24-104">How to: Assign Default Bins to Items</span></span>
<span data-ttu-id="9dc24-105">Si utiliza ubicaciones en un almacén, la asignación de ubicaciones genéricas a sus productos puede facilitar el proceso de envío, recepción y movimiento de sus productos.</span><span class="sxs-lookup"><span data-stu-id="9dc24-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="9dc24-106">Cuando se asigna una ubicación genérica a un producto, se sugiere esta ubicación cada vez que se inicia una transacción de este producto.</span><span class="sxs-lookup"><span data-stu-id="9dc24-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="9dc24-107">Las ubicaciones genéricas se definen en la ventana **Contenido ubicación**.</span><span class="sxs-lookup"><span data-stu-id="9dc24-107">Default bins are defined in the **Bin Content** window.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="9dc24-108">Asignar una ubicación predeterminada a un producto</span><span class="sxs-lookup"><span data-stu-id="9dc24-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="9dc24-109">Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja trabajo creación contenido ubicación** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="9dc24-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="9dc24-110">Rellene la información del código de ubicación y del artículo para cada ubicación que desee configurar como valor predeterminado para un artículo.</span><span class="sxs-lookup"><span data-stu-id="9dc24-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="9dc24-111">Asegúrese de seleccionar el campo **Predeterminado**.</span><span class="sxs-lookup"><span data-stu-id="9dc24-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="9dc24-112">Seleccione la acción **Crear contenido ubicación**.</span><span class="sxs-lookup"><span data-stu-id="9dc24-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="9dc24-113">Las ubicaciones ya están asignadas a su producto.</span><span class="sxs-lookup"><span data-stu-id="9dc24-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9dc24-114">Cuando se ubica un producto, si el producto no tiene asignada una ubicación genérica, se asignará aquélla en la que se ubique como genérica.</span><span class="sxs-lookup"><span data-stu-id="9dc24-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="9dc24-115">Para cambiar las ubicaciones predefinidas de los productos</span><span class="sxs-lookup"><span data-stu-id="9dc24-115">To change the default bin for an item</span></span>  
<span data-ttu-id="9dc24-116">Puede que tenga que cambiar la asignación de la ubicación predeterminada de un artículo o que tenga que asignar una ubicación predeterminada a un artículo nuevo.</span><span class="sxs-lookup"><span data-stu-id="9dc24-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="9dc24-117">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Contenidos ubicación** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="9dc24-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9dc24-118">En el campo **Filtro almacén**, seleccione el código de almacén correspondiente.</span><span class="sxs-lookup"><span data-stu-id="9dc24-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="9dc24-119">Busque el movimiento de contenido de ubicación actual del producto y desactive la casilla **Genérica**.</span><span class="sxs-lookup"><span data-stu-id="9dc24-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="9dc24-120">Busque la línea de contenido de la ubicación que desea que sea la nueva ubicación genérica.</span><span class="sxs-lookup"><span data-stu-id="9dc24-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="9dc24-121">Seleccione la casilla de verificación **Ubicación predeterminada**.</span><span class="sxs-lookup"><span data-stu-id="9dc24-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9dc24-122">Cuando se ubica un producto por primera vez, si el producto no tienen asignada una ubicación genérica, el programa asignará la ubicación como ubicación genérica del producto.</span><span class="sxs-lookup"><span data-stu-id="9dc24-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9dc24-123">Consulte también</span><span class="sxs-lookup"><span data-stu-id="9dc24-123">See Also</span></span>  
[<span data-ttu-id="9dc24-124">Gestión almacén</span><span class="sxs-lookup"><span data-stu-id="9dc24-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="9dc24-125">Grupos contables inventario</span><span class="sxs-lookup"><span data-stu-id="9dc24-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="9dc24-126">[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="9dc24-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="9dc24-127">[Gestión de ensamblaje](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="9dc24-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="9dc24-128">Detalles de diseño: Gestión de almacén</span><span class="sxs-lookup"><span data-stu-id="9dc24-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="9dc24-129">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9dc24-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
