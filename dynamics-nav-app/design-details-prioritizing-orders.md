---
title: "Detalles de diseño: Prioridad de pedidos"
description: "Leer información sobre cómo dar prioridad para satisfacer los requisitos de demanda y oferta."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c01ad1bb74e01ff81f35159865eddf14e9a34910
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="79ce2-103">Detalles de diseño: Prioridad de pedidos</span><span class="sxs-lookup"><span data-stu-id="79ce2-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="79ce2-104">En una UA concreta, la fecha solicitada o disponible representa la máxima prioridad; la demanda de hoy se debe tratar antes que la de la semana que viene.</span><span class="sxs-lookup"><span data-stu-id="79ce2-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="79ce2-105">Pero además de esta prioridad general, el sistema de planificación sugerirá también el tipo de demanda que debe ser satisfecho antes de cubrir otra demanda.</span><span class="sxs-lookup"><span data-stu-id="79ce2-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="79ce2-106">Del mismo modo, sugerirá el origen de suministro que se debe aplicar antes de aplicar otros orígenes de suministro.</span><span class="sxs-lookup"><span data-stu-id="79ce2-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="79ce2-107">Esto se realice según las prioridades de pedido.</span><span class="sxs-lookup"><span data-stu-id="79ce2-107">This is done according to order priorities.</span></span>  
  
<span data-ttu-id="79ce2-108">La demanda y el suministro cargados contribuyen a un perfil del inventario proyectado según las prioridades siguientes:</span><span class="sxs-lookup"><span data-stu-id="79ce2-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  
  
## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="79ce2-109">Prioridades en la demanda</span><span class="sxs-lookup"><span data-stu-id="79ce2-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="79ce2-110">Ya enviado: movimiento de producto</span><span class="sxs-lookup"><span data-stu-id="79ce2-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="79ce2-111">Pedido devolución compra</span><span class="sxs-lookup"><span data-stu-id="79ce2-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="79ce2-112">Pedido venta</span><span class="sxs-lookup"><span data-stu-id="79ce2-112">Sales Order</span></span>  
4. <span data-ttu-id="79ce2-113">Pedido servicio</span><span class="sxs-lookup"><span data-stu-id="79ce2-113">Service Order</span></span>  
5. <span data-ttu-id="79ce2-114">Necesidad de componentes de producción</span><span class="sxs-lookup"><span data-stu-id="79ce2-114">Production Component Need</span></span>  
6. <span data-ttu-id="79ce2-115">Línea de pedido ensamblado</span><span class="sxs-lookup"><span data-stu-id="79ce2-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="79ce2-116">Pedido de transferencia de salida</span><span class="sxs-lookup"><span data-stu-id="79ce2-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="79ce2-117">Pedido abierto (que no ha sido consumido todavía por los pedidos de venta relacionados)</span><span class="sxs-lookup"><span data-stu-id="79ce2-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="79ce2-118">Previsión (que no han consumido aún otros pedidos de venta)</span><span class="sxs-lookup"><span data-stu-id="79ce2-118">Forecast (that has not already been consumed by other sales orders)</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="79ce2-119">Las devoluciones de compras normalmente no intervienen en la planificación de suministros; siempre se deben reservar del lote que se va a devolver.</span><span class="sxs-lookup"><span data-stu-id="79ce2-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="79ce2-120">Si no reserva, las devoluciones de compra desempeñan una función en la disponibilidad y se les da una elevada prioridad para evitar que el sistema de planificación sugiera un pedido de aprovisionamiento solo para servir a una devolución de compra.</span><span class="sxs-lookup"><span data-stu-id="79ce2-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  
  
## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="79ce2-121">Prioridades en el suministro</span><span class="sxs-lookup"><span data-stu-id="79ce2-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="79ce2-122">Ya en el inventario: movimiento de producto (flexibilidad de planificación = ninguna)</span><span class="sxs-lookup"><span data-stu-id="79ce2-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="79ce2-123">Pedido de devolución de venta (flexibilidad de planificación = ninguna)</span><span class="sxs-lookup"><span data-stu-id="79ce2-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="79ce2-124">Pedido de transferencia de entrada</span><span class="sxs-lookup"><span data-stu-id="79ce2-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="79ce2-125">Orden producción</span><span class="sxs-lookup"><span data-stu-id="79ce2-125">Production Order</span></span>  
5. <span data-ttu-id="79ce2-126">Pedido de ensamblado</span><span class="sxs-lookup"><span data-stu-id="79ce2-126">Assembly Order</span></span>  
6. <span data-ttu-id="79ce2-127">Pedido compra</span><span class="sxs-lookup"><span data-stu-id="79ce2-127">Purchase Order</span></span>  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="79ce2-128">Prioridad relacionada con el estado de la demanda y del suministro</span><span class="sxs-lookup"><span data-stu-id="79ce2-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="79ce2-129">Aparte de las prioridades dadas por el tipo de demanda y aprovisionamiento, el estado actual de los pedidos en el proceso de ejecución también define una prioridad.</span><span class="sxs-lookup"><span data-stu-id="79ce2-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="79ce2-130">Por ejemplo, las actividades de almacén repercuten y se tiene en cuenta el estado de los pedidos de ventas, compra, transferencia, ensamblado y órdenes de producción.</span><span class="sxs-lookup"><span data-stu-id="79ce2-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  
  
1. <span data-ttu-id="79ce2-131">Parcialmente controlado (flexibilidad de planificación = ninguna)</span><span class="sxs-lookup"><span data-stu-id="79ce2-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="79ce2-132">Ya en proceso en el almacén (flexibilidad de planificación = ninguna)</span><span class="sxs-lookup"><span data-stu-id="79ce2-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="79ce2-133">Lanzados: todos los tipos de pedido (flexibilidad de planificación = ilimitada)</span><span class="sxs-lookup"><span data-stu-id="79ce2-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="79ce2-134">Orden de producción planificada en firme (flexibilidad de planificación = ilimitada)</span><span class="sxs-lookup"><span data-stu-id="79ce2-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="79ce2-135">Planificado/Abierto: todos los tipos de pedido (flexibilidad de planificación = ilimitada)</span><span class="sxs-lookup"><span data-stu-id="79ce2-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="79ce2-136">Consulte también</span><span class="sxs-lookup"><span data-stu-id="79ce2-136">See Also</span></span>  
<span data-ttu-id="79ce2-137">[Detalles de diseño: Equilibrio de aprovisionamiento y demanda](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="79ce2-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="79ce2-138">[Detalles de diseño: Conceptos centrales del sistema de planificación](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="79ce2-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="79ce2-139">Detalles de diseño: Planificación de aprovisionamiento</span><span class="sxs-lookup"><span data-stu-id="79ce2-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)