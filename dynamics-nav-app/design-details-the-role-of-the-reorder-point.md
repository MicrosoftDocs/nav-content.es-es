---
title: "Detalles de diseño: Función del punto de pedido"
description: "En este tema se destaca la importancia de establecer el punto de pedido, de forma que sepa cuándo solicitar más inventario."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="ee7ae-103">Detalles de diseño: Función del punto de pedido</span><span class="sxs-lookup"><span data-stu-id="ee7ae-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="ee7ae-104">Además del equilibrado general de la oferta y la demanda, el sistema de planificación debe supervisar los niveles de inventario para que los productos afectados respeten las directivas de pedido definidas.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  
  
<span data-ttu-id="ee7ae-105">Un punto de pedido representa la demanda durante un plazo de entrega.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="ee7ae-106">Cuando el inventario proyectado está por debajo del nivel de inventario definido por el punto de pedido, ha llegado el momento de pedir más cantidad.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="ee7ae-107">Mientras tanto, se prevé que el inventario se reduzca gradualmente y posiblemente alcance cero (o el nivel de stock de seguridad), hasta que llegue la reposición.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  
  
<span data-ttu-id="ee7ae-108">Por consiguiente, el sistema de planificación sugerirá un pedido de suministros de programación anticipada en el momento en el que el inventario proyectado quede por debajo del punto de reaprovisionamiento.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  
  
<span data-ttu-id="ee7ae-109">El punto de pedido refleja un determinado nivel de inventario.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="ee7ae-110">No obstante, los niveles de inventario pueden variar significativamente durante el ciclo y, por tanto, el sistema de planificación debe supervisar constantemente el inventario disponible proyectado.</span><span class="sxs-lookup"><span data-stu-id="ee7ae-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="ee7ae-111">Consulte también</span><span class="sxs-lookup"><span data-stu-id="ee7ae-111">See Also</span></span>  
<span data-ttu-id="ee7ae-112">[Detalles de diseño: Directivas de reaprovisionamiento](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="ee7ae-112">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="ee7ae-113">[Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="ee7ae-113">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="ee7ae-114">[Detalles de diseño: Gestión de directivas de reaprovisionamiento](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="ee7ae-114">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="ee7ae-115">Detalles de diseño: Planificación de aprovisionamiento</span><span class="sxs-lookup"><span data-stu-id="ee7ae-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)