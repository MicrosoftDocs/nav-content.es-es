---
title: "Procedimiento: configurar origen y destinos de asignación"
description: "Cada asignación está formada por un origen de asignación y uno o varios destinos de asignación. El origen de asignación define qué costes se asignarán. Los destinos de asignación determinan dónde se deben asignar los costes."
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
ms.openlocfilehash: 91adabefc3e0b4a69b24b34a084f89c17711d573
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-allocation-source-and-targets"></a><span data-ttu-id="ce283-105">Procedimiento: configurar origen y destinos de asignación</span><span class="sxs-lookup"><span data-stu-id="ce283-105">How to: Set Up Allocation Source and Targets</span></span>
<span data-ttu-id="ce283-106">Cada asignación está formada por un origen de asignación y uno o varios destinos de asignación.</span><span class="sxs-lookup"><span data-stu-id="ce283-106">Each allocation consists of an allocation source and one or more allocation targets.</span></span> <span data-ttu-id="ce283-107">El origen de asignación define qué costes se asignarán.</span><span class="sxs-lookup"><span data-stu-id="ce283-107">The allocation source defines which costs will be allocated.</span></span> <span data-ttu-id="ce283-108">Los destinos de asignación determinan dónde se deben asignar los costes.</span><span class="sxs-lookup"><span data-stu-id="ce283-108">The allocation targets determine where the costs will be allocated.</span></span>  

## <a name="to-set-up-cost-allocations"></a><span data-ttu-id="ce283-109">Para configurar asignaciones de coste</span><span class="sxs-lookup"><span data-stu-id="ce283-109">To set up cost allocations</span></span>  
1.  <span data-ttu-id="ce283-110">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Asignación costes** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="ce283-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocation**, and then chose the related link.</span></span>  
2.  <span data-ttu-id="ce283-111">En la ventana **Asignación costes**, elija la acción **Editar**.</span><span class="sxs-lookup"><span data-stu-id="ce283-111">In the **Cost Allocation** window, choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="ce283-112">Especifique un identificador para el origen de asignación en el campo **ID**.</span><span class="sxs-lookup"><span data-stu-id="ce283-112">Enter an ID for the allocation source in the **ID** field.</span></span>  
4.  <span data-ttu-id="ce283-113">Defina un nivel como un número entre 1 y 99 en el campo **Nivel**.</span><span class="sxs-lookup"><span data-stu-id="ce283-113">Define a level as a number between 1 and 99 in the **Level** field.</span></span> <span data-ttu-id="ce283-114">El registro de la asignación seguirá el orden de los niveles.</span><span class="sxs-lookup"><span data-stu-id="ce283-114">The allocation posting will follow the order of the levels.</span></span>  
5.  <span data-ttu-id="ce283-115">Escriba un tipo de coste para definir qué tipos de coste se asignarán en el campo **Intervalo tipo coste**.</span><span class="sxs-lookup"><span data-stu-id="ce283-115">Enter a cost type to define which cost types will be allocated in the **Cost Type Range** field.</span></span> <span data-ttu-id="ce283-116">Si todos los costes de un tipo de coste se asignan, no se define ningún intervalo.</span><span class="sxs-lookup"><span data-stu-id="ce283-116">If all costs for a cost type are allocated, no range is defined.</span></span>  
6.  <span data-ttu-id="ce283-117">Especifique un centro de coste junto con los costes que se asignarán en el campo **Código centro coste**.</span><span class="sxs-lookup"><span data-stu-id="ce283-117">Enter a cost center together with costs to be allocated in the **Cost Center Code** field.</span></span>  
7.  <span data-ttu-id="ce283-118">Especifique un objeto de coste junto con los costes que se asignarán en el campo **Código objeto coste**.</span><span class="sxs-lookup"><span data-stu-id="ce283-118">Enter a cost object together with costs to be allocated in the **Cost Object Code** field.</span></span> <span data-ttu-id="ce283-119">Muy a menudo, este campo permanece vacío porque raramente los objetos de coste se asignan a otros objetos de coste.</span><span class="sxs-lookup"><span data-stu-id="ce283-119">Most often, this field stays empty, because cost objects are rarely allocated to other cost objects.</span></span>  
8.  <span data-ttu-id="ce283-120">Especifique un tipo de coste en el campo **Abonar en tipo de coste**.</span><span class="sxs-lookup"><span data-stu-id="ce283-120">Enter a cost type in the **Credit to Cost Type** field.</span></span> <span data-ttu-id="ce283-121">Los costes que asignen se abonarán en el tipo de coste de origen.</span><span class="sxs-lookup"><span data-stu-id="ce283-121">The costs that are allocated will be credited to the source cost type.</span></span> <span data-ttu-id="ce283-122">El registro de haber se registrará en el tipo de coste que se indique aquí.</span><span class="sxs-lookup"><span data-stu-id="ce283-122">The credit posting will be posted to the cost type given here.</span></span>  
9. <span data-ttu-id="ce283-123">En la ficha desplegable **Líneas**, define los destinos de asignación.</span><span class="sxs-lookup"><span data-stu-id="ce283-123">On the **Lines** FastTab, define the allocation targets.</span></span> <span data-ttu-id="ce283-124">En la primera línea, escriba un tipo de coste en el campo en el campo **Tipo coste destino**.</span><span class="sxs-lookup"><span data-stu-id="ce283-124">On the first line, enter a cost type in the **Target Cost Type** field.</span></span> <span data-ttu-id="ce283-125">Define a qué tipo de coste se carga la asignación.</span><span class="sxs-lookup"><span data-stu-id="ce283-125">It defines which cost type the allocation is debited to.</span></span>  
10. <span data-ttu-id="ce283-126">En la primera línea, introduzca el primer destino de asignación en el campo **Centro de coste de destino** o el campo **Objeto de coste de destino**.</span><span class="sxs-lookup"><span data-stu-id="ce283-126">On the first line, enter the first allocation target in the **Target Cost Center** field or **Target Cost Object** the field.</span></span> <span data-ttu-id="ce283-127">Estos dos campos definen en qué centro de coste u objeto de coste se carga la asignación.</span><span class="sxs-lookup"><span data-stu-id="ce283-127">These two fields define which cost center or cost object the allocation is debited to.</span></span> <span data-ttu-id="ce283-128">Sólo puede rellenar uno de ellos, pero no los dos.</span><span class="sxs-lookup"><span data-stu-id="ce283-128">You can only fill in one of these fields, but not both.</span></span>  
11. <span data-ttu-id="ce283-129">Repita los mismos pasos en la segunda línea para configurar los destinos de asignación adicionales.</span><span class="sxs-lookup"><span data-stu-id="ce283-129">Repeat the same steps on the second line to set up additional allocation targets.</span></span>  
12. <span data-ttu-id="ce283-130">Una vez configurado el destino y los orígenes de asignación, elija la acción **Calcular clave de asignación** para calcular los valores compartidos totales.</span><span class="sxs-lookup"><span data-stu-id="ce283-130">After you have set up the allocation target and sources, choose the **Calculate Allocation Key** action to calculate the total share values.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ce283-131">Seleccione la casilla **Bloqueado** para desactivar la configuración de asignación.</span><span class="sxs-lookup"><span data-stu-id="ce283-131">Select the **Blocked** check box to deactivate the allocation setup.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ce283-132">Consulte también</span><span class="sxs-lookup"><span data-stu-id="ce283-132">See Also</span></span>  
[<span data-ttu-id="ce283-133">Contabilidad para costes</span><span class="sxs-lookup"><span data-stu-id="ce283-133">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 <span data-ttu-id="ce283-134">[Configuración de filtros para las bases de la asignación dinámica](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="ce283-134">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="ce283-135">[Ejemplo: definición de asignaciones estáticas basadas en la proporción de asignación](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md) </span><span class="sxs-lookup"><span data-stu-id="ce283-135">[Scenario Example: Defining Static Allocations Based on Allocation Ratio](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md) </span></span>  
 <span data-ttu-id="ce283-136">[Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span><span class="sxs-lookup"><span data-stu-id="ce283-136">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span></span>  
 <span data-ttu-id="ce283-137">[Definición y asignación de costes](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="ce283-137">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 [<span data-ttu-id="ce283-138">Terminología en contabilidad de costes</span><span class="sxs-lookup"><span data-stu-id="ce283-138">Terminology in Cost Accounting</span></span>](finance-terminology-in-cost-accounting.md)  
 <span data-ttu-id="ce283-139">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ce283-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
