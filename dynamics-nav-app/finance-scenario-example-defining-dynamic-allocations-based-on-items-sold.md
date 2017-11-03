---
title: "Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos"
description: "Este tema muestra un ejemplo de cómo definir asignaciones mediante el método de asignación dinámica. En el ejemplo, se cambia la asignación dinámica de los costes del centro de coste VENTAS para admitir el nuevo EQUIPO TI del objeto de coste. Los paquetes de EQUIPO TI tienen números de producto en el rango de 8904-W a 8924-W. Utiliza las cifras de ventas del año anterior para calcular el reparto. La asignación se registra al tipo de coste de ayuda 9903."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 0d892099be95d52546d98bf17705df2b19f764c7
ms.contentlocale: es-es
ms.lasthandoff: 10/26/2017

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="f1a1f-107">Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos</span><span class="sxs-lookup"><span data-stu-id="f1a1f-107">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="f1a1f-108">Este tema muestra un ejemplo de cómo definir asignaciones mediante el método de asignación dinámica.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-108">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="f1a1f-109">En el ejemplo, se cambia la asignación dinámica de los costes del centro de coste VENTAS para admitir el nuevo EQUIPO TI del objeto de coste.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-109">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="f1a1f-110">Los paquetes de EQUIPO TI tienen números de producto en el rango de 8904-W a 8924-W.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-110">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="f1a1f-111">Utiliza las cifras de ventas del año anterior para calcular el reparto.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-111">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="f1a1f-112">La asignación se registra al tipo de coste de ayuda 9903.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-112">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f1a1f-113">El ejemplo utiliza los datos de demostración en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f1a1f-113">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="f1a1f-114">Para definir las asignaciones dinámicas basándose en los productos vendidos el año anterior</span><span class="sxs-lookup"><span data-stu-id="f1a1f-114">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="f1a1f-115">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Asignaciones coste** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f1a1f-116">En la ventana **Asignación de costes**, elija la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-116">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="f1a1f-117">En el campo **ID**, presione Entrar o escriba un Id.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-117">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="f1a1f-118">En el campo **Nivel**, introduzca **1**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-118">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="f1a1f-119">Especifique las fechas del período en los campos **Válido desde** y **Válido hasta**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-119">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="f1a1f-120">En el campo **Código centro coste**, introduzca **VENTAS**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-120">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="f1a1f-121">En el campo **Abonar en tipo de coste**, especifique un tipo de coste **9903**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-121">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="f1a1f-122">En el campo **Tipo coste destino**, especifique un tipo de coste **9903**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-122">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="f1a1f-123">En el campo **Objeto de coste de destino**, seleccione **Nuevo** para crear un nuevo EQUIPO TI de objeto de coste y rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-123">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="f1a1f-124">Seleccione **EQUIPO TI**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-124">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="f1a1f-125">Deje en blanco el campo **Centro de coste de destino**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-125">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="f1a1f-126">En el campo **Tipo destino asignación**, seleccione **Todos los costes** para definir cómo se asignan todos los costes acumulados.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-126">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="f1a1f-127">En el campo **Base**, seleccione la base de asignación **Productos vendidos (importe)**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-127">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="f1a1f-128">En el campo **Nº filtro**, especifique **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-128">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="f1a1f-129">En el campo **Filtro fecha vto.**, especifique **Año anterior**.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-129">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="f1a1f-130">Elija la acción **Calcular clave de asignación** para calcular el reparto.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-130">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f1a1f-131"> utiliza las cifras de ventas de ejercicios anteriores para calcular un reparto de 1596,50 DL con el 100 por ciento para los paquetes de EQUIPO TI.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-131"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="f1a1f-132">Esto significa que todos los productos vendidos el año anterior se asignarán al EQUIPO TI del objeto de coste.</span><span class="sxs-lookup"><span data-stu-id="f1a1f-132">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f1a1f-133">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f1a1f-133">See Also</span></span>  
 <span data-ttu-id="f1a1f-134">[Configuración de filtros para las bases de la asignación dinámica](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="f1a1f-134">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="f1a1f-135">[Procedimiento: Configurar origen y destinos de asignación](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="f1a1f-135">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="f1a1f-136">[Definición y asignación de costes](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="f1a1f-136">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="f1a1f-137">[Terminología en contabilidad de costes](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f1a1f-137">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="f1a1f-138">Acerca de la contabilidad de costes</span><span class="sxs-lookup"><span data-stu-id="f1a1f-138">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

