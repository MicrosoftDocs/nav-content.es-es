---
title: "Detalles de diseño: Gestión de inventario negativo proyectado"
description: "El punto de pedido expresa la demanda prevista durante el plazo del producto. Cuando se supera el punto de pedido, ha llegado el momento de pedir más. Pero el inventario proyectado debe ser lo suficientemente grande como para satisfacer la demanda hasta que se reciba el nuevo pedido. Mientras tanto, el stock de seguridad debe satisfacer las fluctuaciones en la demanda hasta un nivel de servicio objetivo."
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
ms.openlocfilehash: 66cf357ccd0489d789ec9c2036734ec9f04aad95
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="d44d2-106">Detalles de diseño: Gestión de inventario negativo proyectado</span><span class="sxs-lookup"><span data-stu-id="d44d2-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="d44d2-107">El punto de pedido expresa la demanda prevista durante el plazo del producto.</span><span class="sxs-lookup"><span data-stu-id="d44d2-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="d44d2-108">Cuando se supera el punto de pedido, ha llegado el momento de pedir más.</span><span class="sxs-lookup"><span data-stu-id="d44d2-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="d44d2-109">Pero el inventario proyectado debe ser lo suficientemente grande como para satisfacer la demanda hasta que se reciba el nuevo pedido.</span><span class="sxs-lookup"><span data-stu-id="d44d2-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="d44d2-110">Mientras tanto, el stock de seguridad debe satisfacer las fluctuaciones en la demanda hasta un nivel de servicio objetivo.</span><span class="sxs-lookup"><span data-stu-id="d44d2-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="d44d2-111">Por tanto, el sistema de planificación considera una emergencia el que una demanda futura no se pueda atender desde el inventario proyectado, o dicho de otro modo, que el inventario proyectado quede en negativo.</span><span class="sxs-lookup"><span data-stu-id="d44d2-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="d44d2-112">El sistema se ocupa de dicha excepción mediante la sugerencia de un nuevo pedido de suministro para satisfacer la parte de la demanda que no se puede satisfacer mediante las existencias u otro suministro.</span><span class="sxs-lookup"><span data-stu-id="d44d2-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="d44d2-113">El tamaño de pedido del nuevo pedido de suministro no tendrá en cuenta el inventario máximo o la cantidad del nuevo pedido. Tampoco tendrá en cuenta los modificadores Cantidad máxima pedido, Cantidad mínima pedido y Múltiplos de pedido.</span><span class="sxs-lookup"><span data-stu-id="d44d2-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="d44d2-114">En su lugar, reflejará la deficiencia exacta.</span><span class="sxs-lookup"><span data-stu-id="d44d2-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="d44d2-115">La línea de planificación para este tipo pedido de suministro mostrará un icono de advertencia de emergencia y, tras la búsqueda, se proporcionará información adicional para comunicar al usuario la situación.</span><span class="sxs-lookup"><span data-stu-id="d44d2-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="d44d2-116">En la ilustración siguiente, el aprovisionamiento D representa un pedido de emergencia que ajustar para inventario negativo.</span><span class="sxs-lookup"><span data-stu-id="d44d2-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 ![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")  

1.  <span data-ttu-id="d44d2-117">El suministro **A**, inventario proyectado inicial, está por debajo del punto de pedido.</span><span class="sxs-lookup"><span data-stu-id="d44d2-117">Supply **A**, initial projected inventory, is below reorder point.</span></span>  

2.  <span data-ttu-id="d44d2-118">Se ha creado un nuevo aprovisionamiento programación de forma anticipada (**C**).</span><span class="sxs-lookup"><span data-stu-id="d44d2-118">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="d44d2-119">(Cantidad = Inventario máximo – Nivel de inventario proyectado)</span><span class="sxs-lookup"><span data-stu-id="d44d2-119">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  

3.  <span data-ttu-id="d44d2-120">El suministro **A** está cerrado por la demanda **B**, que no se cubre por completo.</span><span class="sxs-lookup"><span data-stu-id="d44d2-120">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="d44d2-121">(La demanda **B** podría intentar programar el aprovisionamiento C, pero esto no sucederá según el concepto de ciclo).</span><span class="sxs-lookup"><span data-stu-id="d44d2-121">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  

4.  <span data-ttu-id="d44d2-122">Se crea un nuevo suministro (**D**) para cubrir la cantidad restante de la demanda **B**.</span><span class="sxs-lookup"><span data-stu-id="d44d2-122">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  

5.  <span data-ttu-id="d44d2-123">La demanda **B** está cerrada (creando un aviso al inventario proyectado).</span><span class="sxs-lookup"><span data-stu-id="d44d2-123">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  

6.  <span data-ttu-id="d44d2-124">Se cierra el nuevo suministro **D**.</span><span class="sxs-lookup"><span data-stu-id="d44d2-124">The new supply **D** is closed.</span></span>  

7.  <span data-ttu-id="d44d2-125">Se ha comprobado el inventario proyectado; no se ha superado el punto de pedido.</span><span class="sxs-lookup"><span data-stu-id="d44d2-125">Projected Inventory is checked; reorder point has not been crossed.</span></span>  

8.  <span data-ttu-id="d44d2-126">El suministro **C** está cerrado (no hay más demanda).</span><span class="sxs-lookup"><span data-stu-id="d44d2-126">Supply **C** is closed (no more demand exists).</span></span>  

9. <span data-ttu-id="d44d2-127">Comprobación final: que no queden avisos pendientes en el nivel de inventario.</span><span class="sxs-lookup"><span data-stu-id="d44d2-127">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d44d2-128">El paso 4 refleja cómo reacciona el sistema en versiones anteriores a Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="d44d2-128">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="d44d2-129">De este modo concluye la descripción de los principios básicos relacionados con la planificación de inventario basada en directivas de reorganización.</span><span class="sxs-lookup"><span data-stu-id="d44d2-129">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="d44d2-130">En la sección siguiente se describen las características de las cuatro directivas de reaprovisionamiento admitidas.</span><span class="sxs-lookup"><span data-stu-id="d44d2-130">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d44d2-131">Consulte también</span><span class="sxs-lookup"><span data-stu-id="d44d2-131">See Also</span></span>  
 <span data-ttu-id="d44d2-132">[Detalles de diseño: Directivas de reaprovisionamiento](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d44d2-132">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="d44d2-133">[Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="d44d2-133">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="d44d2-134">[Detalles de diseño: Gestión de directivas de reaprovisionamiento](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d44d2-134">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="d44d2-135">Detalles de diseño: Planificación de aprovisionamiento</span><span class="sxs-lookup"><span data-stu-id="d44d2-135">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
