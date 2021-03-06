---
title: "Detalles de diseño: Función del ciclo"
description: "El propósito del ciclo es recopilar los eventos de demanda dentro del intervalo de tiempo para crear un pedido de suministro conjunto."
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
ms.openlocfilehash: c05bb3ca1913b1f5d0abe0bfa26248d08e080ad6
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-time-bucket"></a>Detalles de diseño: Función del ciclo
El propósito del ciclo es recopilar los eventos de demanda dentro del intervalo de tiempo para crear un pedido de suministro conjunto.  
  
 En el caso de directivas de reaprovisionamiento que utilizan un punto de pedido se puede definir un ciclo. De este modo se garantiza que se acumula la demanda en el mismo periodo de tiempo antes de comprobar el impacto en el inventario proyectado y si se ha superado el último punto de pedido. Si se sobrepasa el punto de pedido, se programa de forma anticipada un nuevo pedido de aprovisionamiento desde el final del periodo definido por el ciclo. Los ciclos comienzan en la fecha inicial de planificación.  
  
 El concepto por ciclos refleja el proceso manual de comprobación del nivel de inventario de un modo frecuente en vez de hacerlo por cada transacción. El usuario debe definir la frecuencia (el ciclo). Por ejemplo, el usuario recopila todas las exigencias de producto de un proveedor para hacer un pedido semanal.  
  
 ![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")  
  
 Por lo general, el ciclo se usa para evitar un efecto de cascada. Por ejemplo, una fila equilibrada de demanda y aprovisionamiento donde se cancela una demanda temprana, o se crea una nueva. El resultado podría ser que se programe cada pedido de suministro (sin incluir el último).  
  
## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Directivas de reaprovisionamiento](design-details-reordering-policies.md)   
 [Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md)   
 [Detalles de diseño: Gestión de directivas de reaprovisionamiento](design-details-handling-reordering-policies.md)   
 [Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)
