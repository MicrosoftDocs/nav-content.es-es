---
title: "Configurar plantillas de ubicación"
description: "Con la funcionalidad de ubicación y picking directo, se sugiere la ubicación más adecuada para los productos en un momento determinado, según la plantilla de ubicación que ha configurado para el almacén, los rankings que ha dado a las ubicaciones y las cantidades máxima y mínima que ha definido para las ubicaciones fijas."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: be51b4d1cfc4d2a54e5f44f6419ed4539c01e9df
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-put-away-templates"></a><span data-ttu-id="dcde9-103">Cómo configurar plantillas de ubicación</span><span class="sxs-lookup"><span data-stu-id="dcde9-103">How to: Set Up Put-away Templates</span></span>
<span data-ttu-id="dcde9-104">Con la funcionalidad de ubicación y picking directo, se sugiere la ubicación más adecuada para los productos en un momento determinado, según la plantilla de ubicación que ha configurado para el almacén, los rankings que ha dado a las ubicaciones y las cantidades máxima y mínima que ha definido para las ubicaciones fijas.</span><span class="sxs-lookup"><span data-stu-id="dcde9-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="dcde9-105">Puede configurar varias plantillas de ubicación y seleccionar una para controlar las ubicaciones en general en el almacén.</span><span class="sxs-lookup"><span data-stu-id="dcde9-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="dcde9-106">También puede seleccionar una plantilla de ubicación para cualquier producto o unidad de almacenamiento que tenga unos requisitos de ubicación especiales.</span><span class="sxs-lookup"><span data-stu-id="dcde9-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="dcde9-107">Para configurar las plantillas de ubicación</span><span class="sxs-lookup"><span data-stu-id="dcde9-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="dcde9-108">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plantillas ubicación** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="dcde9-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="dcde9-109">Seleccione la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="dcde9-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="dcde9-110">Escriba un código que sea el identificador exclusivo de la plantilla que va a crear.</span><span class="sxs-lookup"><span data-stu-id="dcde9-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="dcde9-111">Escriba una breve descripción, si lo desea.</span><span class="sxs-lookup"><span data-stu-id="dcde9-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="dcde9-112">Rellene la primera línea con los requisitos de la ubicación que desea que se rellenen en primer lugar cuando se sugiera una ubicación.</span><span class="sxs-lookup"><span data-stu-id="dcde9-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="dcde9-113">Rellene la segunda línea con los requisitos de ubicación que serán la segunda opción a seguir para utilizar esta ubicación.</span><span class="sxs-lookup"><span data-stu-id="dcde9-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="dcde9-114">El programa sólo se utilizará si no encuentra una ubicación que cumpla los requisitos de la primera línea.</span><span class="sxs-lookup"><span data-stu-id="dcde9-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="dcde9-115">Continúe rellenando las líneas hasta que haya descrito todos los lugares de ubicación adecuados que desea utilizar en el proceso de ubicación.</span><span class="sxs-lookup"><span data-stu-id="dcde9-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="dcde9-116">En la última línea de la plantilla de ubicación, seleccione la casilla **Busca ubicación aleatoria**.</span><span class="sxs-lookup"><span data-stu-id="dcde9-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="dcde9-117">Puede crear varias plantillas de ubicación y, a continuación, aplicarlas como necesite.</span><span class="sxs-lookup"><span data-stu-id="dcde9-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="dcde9-118">Se utilizará primero la plantilla de ubicación que ha seleccionado para el producto o unidad de almacenamiento, si existe.</span><span class="sxs-lookup"><span data-stu-id="dcde9-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="dcde9-119">Si estos campos no están rellenos, se utilizará la plantilla que ha seleccionado para el almacén en la ficha desplegable **Políticas ubic.** de la ficha de almacén.</span><span class="sxs-lookup"><span data-stu-id="dcde9-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="dcde9-120">Consulte también</span><span class="sxs-lookup"><span data-stu-id="dcde9-120">See Also</span></span>  
[<span data-ttu-id="dcde9-121">Gestión almacén</span><span class="sxs-lookup"><span data-stu-id="dcde9-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="dcde9-122">Grupos contables inventario</span><span class="sxs-lookup"><span data-stu-id="dcde9-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="dcde9-123">[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="dcde9-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="dcde9-124">[Gestión de ensamblaje](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="dcde9-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="dcde9-125">Detalles de diseño: Gestión de almacén</span><span class="sxs-lookup"><span data-stu-id="dcde9-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="dcde9-126">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dcde9-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
