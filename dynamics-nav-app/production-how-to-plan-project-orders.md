---
title: "Procedimiento: Planifique las órdenes de proyecto"
description: "Esta tarea de planificación se inicia desde un pedido de venta y utiliza la ventana **Planificación pedido venta**. Una vez creada la orden de producción de un proyecto, puede seguir planificándola en la ventana **Planificación de pedidos**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a03cdaf16b25cbcf030e9a33c538ea3df96a1fe9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-project-orders"></a><span data-ttu-id="0a3d7-104">Procedimiento: Planifique las órdenes de proyecto</span><span class="sxs-lookup"><span data-stu-id="0a3d7-104">How to: Plan Project Orders</span></span>
<span data-ttu-id="0a3d7-105">Esta tarea de planificación se inicia desde un pedido de venta y utiliza la ventana **Planificación pedido venta**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-105">This planning task starts from a sales order and uses the **Sales Order Planning** window.</span></span> <span data-ttu-id="0a3d7-106">Una vez creada la orden de producción de un proyecto, puede seguir planificándola en la ventana **Planificación de pedidos**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-106">Once you have created a project production order, you can plan it further by using the **Order Planning** window.</span></span>  

## <a name="to-create-a-project-production-order"></a><span data-ttu-id="0a3d7-107">Para crear una orden de producción de un proyecto</span><span class="sxs-lookup"><span data-stu-id="0a3d7-107">To create a project production order</span></span>  

1.  <span data-ttu-id="0a3d7-108">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0a3d7-109">Seleccione el pedido de venta que representa el proyecto de producción y después seleccione la acción **Planificación**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-109">Select the sales order that represents the production project, and then choose the **Planning** action.</span></span>  
4.  <span data-ttu-id="0a3d7-110">En la ventana **Planificación de pedido de venta**, seleccione la acción **Crear orden de producción**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-110">In the **Sales Order Planning** window, choose  the **Create Prod. Order** action.</span></span>  
5.  <span data-ttu-id="0a3d7-111">En la ventana **Crear pedido a partir de las ventas**, en el campo **Tipo orden**, seleccione **Orden proyecto**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-111">In the **Create Order from Sales** window, in the **Order Type** field, select **Project Order**.</span></span>  
6.  <span data-ttu-id="0a3d7-112">Elija el botón **Sí**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-112">Choose the **Yes** button.</span></span>  
7.  <span data-ttu-id="0a3d7-113">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Órdenes de producción** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production Orders**, and then choose the related link.</span></span>
8. <span data-ttu-id="0a3d7-114">Abra la orden de producción que acaba de crear.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-114">Open the production order just created.</span></span>  

    <span data-ttu-id="0a3d7-115">Tenga en cuenta que el campo **Tipo de procedencia** de la orden de producción contiene **Cabecera de ventas** y la orden tiene varias líneas, una para cada producto de línea de venta que debe fabricarse.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-115">Notice that the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span></span>  
9. <span data-ttu-id="0a3d7-116">Seleccione la acción **Planificación**.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-116">Choose the **Planning** action.</span></span>
10. <span data-ttu-id="0a3d7-117">En la ventana **Planificación de pedidos**, seleccione la acción **Actualizar** para calcular una nueva demanda.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-117">In the **Order Planning** window, choose the **Refresh** action to calculate new demand.</span></span>  

<span data-ttu-id="0a3d7-118">Se mostrará la línea de cabecera de la orden del proyecto con todas las líneas de demanda no satisfecha expandidas bajo ella.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-118">The order header line for the project order is displayed with all unfulfilled demand lines expanded under it.</span></span> <span data-ttu-id="0a3d7-119">Aunque la orden de producción contiene líneas para varios productos fabricados, la demanda total de todas las líneas de la orden de producción aparece bajo una línea de cabecera de la orden en la ventana **Programación de pedidos** y se muestra el nombre del cliente original.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-119">Although the production order contains lines for several produced items, the total demand for all production order lines is listed under one order header line in the **Order Planning** window, and the original customer name is displayed.</span></span> <span data-ttu-id="0a3d7-120">Ahora puede empezar a planificar la demanda, según se indica en [Planificación de una nueva demanda pedido por pedido](production-how-to-plan-for-new-demand.md).</span><span class="sxs-lookup"><span data-stu-id="0a3d7-120">You can now proceed to plan for the demand as described in [How to: Plan for New Demand Order by Order](production-how-to-plan-for-new-demand.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0a3d7-121">Las líneas de demanda en el orden de producción del proyecto que disponen de **Prod. Pedido** en el campo de **Sistema reposición** representan las órdenes de producción subyacentes.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-121">Demand lines in the project production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span></span> <span data-ttu-id="0a3d7-122">Después de generar estas órdenes de producción, deberá volver a calcular un plan en la ventana **Programación de pedidos** para identificar la demanda de componentes no satisfecha.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-122">After you have generated these production orders, you must again calculate a plan in the **Order Planning** window to identify any unfulfilled component demand for them.</span></span> <span data-ttu-id="0a3d7-123">En ese caso, estas líneas se muestran como líneas de demanda bajo una línea de cabecera de orden de producción normal, es decir, la relación del proyecto ya no se muestra en la ventana.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-123">In that case, they are displayed as demand lines under a normal production order header line, meaning, the project relation is no longer visible in the window.</span></span> <span data-ttu-id="0a3d7-124">Sin embargo, si utiliza la función Seguimiento pedido, puede retroceder y avanzar por todos los pedidos de suministro creados bajo el pedido de venta original.</span><span class="sxs-lookup"><span data-stu-id="0a3d7-124">However, if you are using the Order Tracking feature, then you can look back and forth to all supply orders made under the original sales order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0a3d7-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="0a3d7-125">See Also</span></span>
<span data-ttu-id="0a3d7-126">[Planificación](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="0a3d7-126">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="0a3d7-127">Configuración de fabricación</span><span class="sxs-lookup"><span data-stu-id="0a3d7-127">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="0a3d7-128">[Fabricación](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="0a3d7-128">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="0a3d7-129">Grupos contables inventario</span><span class="sxs-lookup"><span data-stu-id="0a3d7-129">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0a3d7-130">Compras</span><span class="sxs-lookup"><span data-stu-id="0a3d7-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0a3d7-131">[Detalles de diseño: planificación de aprovisionamiento](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="0a3d7-131">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="0a3d7-132">Procedimientos recomendados de configuración: planificación de suministros</span><span class="sxs-lookup"><span data-stu-id="0a3d7-132">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="0a3d7-133">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0a3d7-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
