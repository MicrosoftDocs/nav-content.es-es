---
title: "Definición y asignación de costes"
description: Las asignaciones de costes mueven los costes e ingresos entre tipos de coste, centros de coste y objetos de coste. Puede definir tantas asignaciones como necesite.
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
ms.openlocfilehash: f7c34e8f4c57e2effc03b8dcd2a722d7bdbb4692
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="f1975-104">Definición y asignación de costes</span><span class="sxs-lookup"><span data-stu-id="f1975-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="f1975-105">Las asignaciones de costes mueven los costes e ingresos entre tipos de coste, centros de coste y objetos de coste.</span><span class="sxs-lookup"><span data-stu-id="f1975-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="f1975-106">Puede definir tantas asignaciones como necesite.</span><span class="sxs-lookup"><span data-stu-id="f1975-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="f1975-107">Cada asignación consta de:</span><span class="sxs-lookup"><span data-stu-id="f1975-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="f1975-108">Un origen asignación.</span><span class="sxs-lookup"><span data-stu-id="f1975-108">An allocation source.</span></span>  
-   <span data-ttu-id="f1975-109">Uno o varios destinos de asignación.</span><span class="sxs-lookup"><span data-stu-id="f1975-109">One or more allocation targets.</span></span>  

<span data-ttu-id="f1975-110">El origen de asignación establece qué costes se deben asignar, y los destinos de asignación determinan dónde se deben asignar los costes.</span><span class="sxs-lookup"><span data-stu-id="f1975-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="f1975-111">Por ejemplo, un origen de asignación puede ser los costes del tipo de coste Electricidad y Calefacción.</span><span class="sxs-lookup"><span data-stu-id="f1975-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="f1975-112">Asigna todos los costes de electricidad y calefacción a tres centros de coste: Taller, Producción y Ventas.</span><span class="sxs-lookup"><span data-stu-id="f1975-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="f1975-113">Estos centros de coste son los destinos de asignación.</span><span class="sxs-lookup"><span data-stu-id="f1975-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="f1975-114">Para cada origen de asignación, puede definir un nivel de asignación, un periodo de validez y una variante como identificador de grupo.</span><span class="sxs-lookup"><span data-stu-id="f1975-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="f1975-115">Puede utilizar un trabajo por lotes para definir filtros para seleccionar definiciones de asignación y luego ejecutar asignaciones de coste automáticamente.</span><span class="sxs-lookup"><span data-stu-id="f1975-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="f1975-116">Para cada destino de asignación, define una base de asignaciones.</span><span class="sxs-lookup"><span data-stu-id="f1975-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="f1975-117">La base de la asignaciones puede ser estática o dinámica.</span><span class="sxs-lookup"><span data-stu-id="f1975-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="f1975-118">Las bases de asignaciones estáticas se basan en un valor definido, por ejemplo los metros cuadrados o una proporción de asignación establecida, como 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="f1975-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="f1975-119">Las bases de asignaciones dinámicas se basan en valores cambiables, como el número de empleados de un centro de coste o los ingresos de ventas de un objeto de coste en un determinado periodo de tiempo.</span><span class="sxs-lookup"><span data-stu-id="f1975-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="f1975-120">En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.</span><span class="sxs-lookup"><span data-stu-id="f1975-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="f1975-121">Para</span><span class="sxs-lookup"><span data-stu-id="f1975-121">To</span></span>|<span data-ttu-id="f1975-122">Vea</span><span class="sxs-lookup"><span data-stu-id="f1975-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="f1975-123">Configurar el origen de asignación y sus destinos.</span><span class="sxs-lookup"><span data-stu-id="f1975-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="f1975-124">Procedimiento: configurar origen y destinos de asignación</span><span class="sxs-lookup"><span data-stu-id="f1975-124">How to: Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="f1975-125">Configuración de varios filtros para las bases de la asignaciones dinámicas.</span><span class="sxs-lookup"><span data-stu-id="f1975-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="f1975-126">Configuración de filtros para las bases de la asignación dinámica</span><span class="sxs-lookup"><span data-stu-id="f1975-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="f1975-127">Consulte un ejemplo de cómo definir una asignación estática.</span><span class="sxs-lookup"><span data-stu-id="f1975-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="f1975-128">Ejemplo: definición de asignaciones estáticas basadas en la proporción de asignación</span><span class="sxs-lookup"><span data-stu-id="f1975-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="f1975-129">Consulte un ejemplo de cómo definir una asignación dinámica.</span><span class="sxs-lookup"><span data-stu-id="f1975-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="f1975-130">Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos</span><span class="sxs-lookup"><span data-stu-id="f1975-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="f1975-131">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f1975-131">See Also</span></span>  
 <span data-ttu-id="f1975-132">[Configuración de contabilidad de costes](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f1975-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="f1975-133">[Transferencia y registro de movimientos de coste](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="f1975-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="f1975-134">[Contabilidad para costes](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f1975-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="f1975-135">[Terminología en contabilidad de costes](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f1975-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="f1975-136">Acerca de la contabilidad de costes</span><span class="sxs-lookup"><span data-stu-id="f1975-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)
