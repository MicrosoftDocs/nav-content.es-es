---
title: "Configuración de filtros para las bases de la asignación dinámica"
description: "El método de asignación dinámica se basa en los valores cambiables. Por ejemplo, el número de empleados de un centro de coste o los productos vendidos de un objeto de coste en un periodo de tiempo determinado. Existen nueve bases predefinidas de asignación y doce rangos de fechas dinámicas. Define distintos filtros basados en la base de asignación."
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
ms.openlocfilehash: 8372f855cfaa19456ab597e163006ae20411defd
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="setting-filters-for-dynamic-allocation-bases"></a><span data-ttu-id="9b81a-106">Configuración de filtros para las bases de la asignación dinámica</span><span class="sxs-lookup"><span data-stu-id="9b81a-106">Setting Filters for Dynamic Allocation Bases</span></span>
<span data-ttu-id="9b81a-107">El método de asignación dinámica se basa en los valores cambiables.</span><span class="sxs-lookup"><span data-stu-id="9b81a-107">The dynamic allocation method is based on changeable values.</span></span> <span data-ttu-id="9b81a-108">Por ejemplo, el número de empleados de un centro de coste o los productos vendidos de un objeto de coste en un periodo de tiempo determinado.</span><span class="sxs-lookup"><span data-stu-id="9b81a-108">For example, the number of employees in a cost center or the items sold of a cost object in a specific time period.</span></span> <span data-ttu-id="9b81a-109">Existen nueve bases predefinidas de asignación y doce rangos de fechas dinámicas.</span><span class="sxs-lookup"><span data-stu-id="9b81a-109">There are nine pre-defined allocation bases and twelve dynamic date ranges.</span></span> <span data-ttu-id="9b81a-110">Define distintos filtros basados en la base de asignación.</span><span class="sxs-lookup"><span data-stu-id="9b81a-110">You set different filters based on the allocation base.</span></span>  

## <a name="setting-filters-for-dynamic-allocation-bases"></a><span data-ttu-id="9b81a-111">Configuración de filtros para las bases de la asignación dinámica</span><span class="sxs-lookup"><span data-stu-id="9b81a-111">Setting Filters for Dynamic Allocation Bases</span></span>  
 <span data-ttu-id="9b81a-112">La siguiente tabla muestra qué filtros son posibles para distintas bases de asignación y qué valores son válidos en los campos **Filtro nº** y **Filtro grupo**.</span><span class="sxs-lookup"><span data-stu-id="9b81a-112">The following table shows which filters are possible for different allocation bases and which values are valid in the **No. Filter** and **Group Filter** fields.</span></span> <span data-ttu-id="9b81a-113">Presione F1 en el campo **Filtro fecha vto.** para leer descripciones detalladas.</span><span class="sxs-lookup"><span data-stu-id="9b81a-113">Press F1 in the **Date Filter Code** field to read detailed descriptions.</span></span>  

|<span data-ttu-id="9b81a-114">**Base**</span><span class="sxs-lookup"><span data-stu-id="9b81a-114">**Base**</span></span>|<span data-ttu-id="9b81a-115">**Filtro Nº**</span><span class="sxs-lookup"><span data-stu-id="9b81a-115">**No. Filter**</span></span>|<span data-ttu-id="9b81a-116">**Filtro fecha vto.**</span><span class="sxs-lookup"><span data-stu-id="9b81a-116">**Date Filter Code**</span></span>|<span data-ttu-id="9b81a-117">**Filtro centro coste**</span><span class="sxs-lookup"><span data-stu-id="9b81a-117">**Cost Center Filter**</span></span>|<span data-ttu-id="9b81a-118">**Filtro objeto coste**</span><span class="sxs-lookup"><span data-stu-id="9b81a-118">**Cost Object Filter**</span></span>|<span data-ttu-id="9b81a-119">**Filtro grupo**</span><span class="sxs-lookup"><span data-stu-id="9b81a-119">**Group Filter**</span></span>|  
|--------------|----------------------------------------|----------------------------------------------|------------------------------------------------|------------------------------------------------|------------------------------------------|  
|<span data-ttu-id="9b81a-120">Movimientos de contabilidad</span><span class="sxs-lookup"><span data-stu-id="9b81a-120">G/L Entries</span></span>|<span data-ttu-id="9b81a-121">Cuenta</span><span class="sxs-lookup"><span data-stu-id="9b81a-121">G/L Account</span></span>|<span data-ttu-id="9b81a-122">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-122">Yes</span></span>|<span data-ttu-id="9b81a-123">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-123">Yes</span></span>|<span data-ttu-id="9b81a-124">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-124">Yes</span></span>|<span data-ttu-id="9b81a-125">N/D</span><span class="sxs-lookup"><span data-stu-id="9b81a-125">N/A</span></span>|  
|<span data-ttu-id="9b81a-126">Movs. pptos. contabilidad</span><span class="sxs-lookup"><span data-stu-id="9b81a-126">G/L Budget Entries</span></span>|<span data-ttu-id="9b81a-127">Cuenta</span><span class="sxs-lookup"><span data-stu-id="9b81a-127">G/L Account</span></span>|<span data-ttu-id="9b81a-128">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-128">Yes</span></span>|<span data-ttu-id="9b81a-129">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-129">Yes</span></span>|<span data-ttu-id="9b81a-130">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-130">Yes</span></span>|<span data-ttu-id="9b81a-131">Nombres pptos. contabilidad</span><span class="sxs-lookup"><span data-stu-id="9b81a-131">G/L Budget Name</span></span>|  
|<span data-ttu-id="9b81a-132">Movimientos de tipo de coste</span><span class="sxs-lookup"><span data-stu-id="9b81a-132">Cost Type Entries</span></span>|<span data-ttu-id="9b81a-133">Tipo de coste</span><span class="sxs-lookup"><span data-stu-id="9b81a-133">Cost Type</span></span>|<span data-ttu-id="9b81a-134">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-134">Yes</span></span>|<span data-ttu-id="9b81a-135">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-135">Yes</span></span>|<span data-ttu-id="9b81a-136">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-136">Yes</span></span>|<span data-ttu-id="9b81a-137">N/D</span><span class="sxs-lookup"><span data-stu-id="9b81a-137">N/A</span></span>|  
|<span data-ttu-id="9b81a-138">Movs. ppto. costes</span><span class="sxs-lookup"><span data-stu-id="9b81a-138">Cost Budget Entries</span></span>|<span data-ttu-id="9b81a-139">Tipo de coste</span><span class="sxs-lookup"><span data-stu-id="9b81a-139">Cost Type</span></span>|<span data-ttu-id="9b81a-140">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-140">Yes</span></span>|<span data-ttu-id="9b81a-141">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-141">Yes</span></span>|<span data-ttu-id="9b81a-142">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-142">Yes</span></span>|<span data-ttu-id="9b81a-143">Nombre ppto.</span><span class="sxs-lookup"><span data-stu-id="9b81a-143">Budget Name</span></span>|  
|<span data-ttu-id="9b81a-144">Nº de empleados</span><span class="sxs-lookup"><span data-stu-id="9b81a-144">No of Employees</span></span>|<span data-ttu-id="9b81a-145">N/D</span><span class="sxs-lookup"><span data-stu-id="9b81a-145">N/A</span></span>|<span data-ttu-id="9b81a-146">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-146">Yes</span></span>|<span data-ttu-id="9b81a-147">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-147">Yes</span></span>|<span data-ttu-id="9b81a-148">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-148">Yes</span></span>|<span data-ttu-id="9b81a-149">N/D</span><span class="sxs-lookup"><span data-stu-id="9b81a-149">N/A</span></span>|  
|<span data-ttu-id="9b81a-150">Productos vendidos (cantidad)</span><span class="sxs-lookup"><span data-stu-id="9b81a-150">Items Sold (Qty)</span></span>|<span data-ttu-id="9b81a-151">Nº producto</span><span class="sxs-lookup"><span data-stu-id="9b81a-151">Item No.</span></span>|<span data-ttu-id="9b81a-152">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-152">Yes</span></span>|<span data-ttu-id="9b81a-153">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-153">Yes</span></span>|<span data-ttu-id="9b81a-154">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-154">Yes</span></span>|<span data-ttu-id="9b81a-155">Grupo contable existencias</span><span class="sxs-lookup"><span data-stu-id="9b81a-155">Inventory Posting Group</span></span>|  
|<span data-ttu-id="9b81a-156">Productos comprados (cantidad)</span><span class="sxs-lookup"><span data-stu-id="9b81a-156">Items Purchased (Qty)</span></span>|<span data-ttu-id="9b81a-157">Nº producto</span><span class="sxs-lookup"><span data-stu-id="9b81a-157">Item No.</span></span>|<span data-ttu-id="9b81a-158">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-158">Yes</span></span>|<span data-ttu-id="9b81a-159">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-159">Yes</span></span>|<span data-ttu-id="9b81a-160">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-160">Yes</span></span>|<span data-ttu-id="9b81a-161">Grupo contable existencias</span><span class="sxs-lookup"><span data-stu-id="9b81a-161">Inventory Posting Group</span></span>|  
|<span data-ttu-id="9b81a-162">Productos vendidos (importe)</span><span class="sxs-lookup"><span data-stu-id="9b81a-162">Items Sold (Amount)</span></span>|<span data-ttu-id="9b81a-163">Nº producto</span><span class="sxs-lookup"><span data-stu-id="9b81a-163">Item No.</span></span>|<span data-ttu-id="9b81a-164">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-164">Yes</span></span>|<span data-ttu-id="9b81a-165">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-165">Yes</span></span>|<span data-ttu-id="9b81a-166">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-166">Yes</span></span>|<span data-ttu-id="9b81a-167">Grupo contable existencias</span><span class="sxs-lookup"><span data-stu-id="9b81a-167">Inventory Posting Group</span></span>|  
|<span data-ttu-id="9b81a-168">Productos comprados (importe)</span><span class="sxs-lookup"><span data-stu-id="9b81a-168">Items Purchased (Amount)</span></span>|<span data-ttu-id="9b81a-169">N.º producto</span><span class="sxs-lookup"><span data-stu-id="9b81a-169">Item No.</span></span>|<span data-ttu-id="9b81a-170">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-170">Yes</span></span>|<span data-ttu-id="9b81a-171">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-171">Yes</span></span>|<span data-ttu-id="9b81a-172">Sí</span><span class="sxs-lookup"><span data-stu-id="9b81a-172">Yes</span></span>|<span data-ttu-id="9b81a-173">Grupo contable inventario</span><span class="sxs-lookup"><span data-stu-id="9b81a-173">Inventory Posting Group</span></span>|  

## <a name="see-also"></a><span data-ttu-id="9b81a-174">Consulte también</span><span class="sxs-lookup"><span data-stu-id="9b81a-174">See Also</span></span>  
 <span data-ttu-id="9b81a-175">[Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span><span class="sxs-lookup"><span data-stu-id="9b81a-175">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span></span>  
 <span data-ttu-id="9b81a-176">[Procedimiento: Configurar origen y destinos de asignación](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="9b81a-176">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 [<span data-ttu-id="9b81a-177">Definición y asignación de costes</span><span class="sxs-lookup"><span data-stu-id="9b81a-177">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)
