---
title: "Cómo hacer un seguimiento de las relaciones entre demanda y suministro"
description: "Desde cualquier documento de suministro o demanda de la llamada red de pedidos, puede efectuar el seguimiento de la demanda de pedido (cantidad seguida), previsión, pedido de ventas abierto o parámetro de planificación (cantidad no seguida) que ha dado lugar a la línea de planificación en cuestión."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: acf030ab57c9251671900b1262dd8441c241c185
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-track-relations-between-demand-and-supply"></a>Cómo hacer un seguimiento de las relaciones entre demanda y suministro
Desde cualquier documento de suministro o demanda de la llamada red de pedidos, puede efectuar el seguimiento de la demanda de pedido (cantidad seguida), previsión, pedido de ventas abierto o parámetro de planificación (cantidad no seguida) que ha dado lugar a la línea de planificación en cuestión.

Las hojas de planificación también presentan información de planificación complementaria, acerca de entidades sin pedidos para ayudar al planificador a elaborar un plan de suministro óptimo. Para obtener más información, consulte la sección "Elementos de planificación sin seguimiento".

## <a name="to-track-linked-items"></a>Para seguir productos relacionados
El seguimiento de pedidos muestra cómo se relacionan los pedidos de venta, las órdenes de producción y los pedidos de compra con las órdenes de fabricación en los sistemas de planificación y reservas.

A continuación se describe cómo seguir productos asociados en una orden de producción planificada en firme. Los pasos son parecidos a los de todos los tipos de pedidos y planificación de las líneas de hoja de trabajo.

1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), especifique **O.P. Planificada en firme** y elija el vínculo relacionado.
2. Abra la orden de producción planificada en firme pertinente de la lista.
3. En la ficha desplegable **Líneas**, elija la acción **Funciones** y, a continuación, seleccione la acción **Seguimiento de pedido**.

Las líneas de **Seguimiento de pedido** muestran los documentos que están relacionados con la línea de pedido de producción actual.

## <a name="untracked-planning-elements"></a>Elementos planificación sin seguimiento
Se abre la ventana **Elementos de planificación sin seguimiento** cuando elige el campo **Cantidad sin seguimiento** en la ventana **Planificación de pedidos**. Responde a dos propósitos:

1. Albergar información sobre cantidades sin seguimiento que se muestran cuando el usuario busca desde la ventana Seguimiento pedido las cantidades sin seguimiento.
2. Albergar los mensajes de advertencia que se muestran cuando el usuario selecciona el icono de **Advertencia** en la ventana **Hoja de planificación**.

La ventana contiene entradas que contabilizan la cantidad de excedentes sin seguimiento con el objeto de realizar un seguimiento de la red. Estas entradas se generan durante la ejecución de la planificación y explican la procedencia de dicha cantidad en las líneas de seguimiento de pedido. La procedencia de este excedente sin seguimiento puede ser:

- Previsión de producción
- Pedidos abiertos
- Stock de seguridad
- Punto de pedido
- Stock máximo
- Cantidad a solicitar
- Cantidad máxima pedido
- Cantidad mínima pedido
- Múltiplos de pedido
- Amort. (% tamaño lote)

## <a name="see-also"></a>Consulte también  
[Planificación](production-planning.md)   
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Detalles de diseño: Reserva, seguimiento y mensajes de acciones](design-details-reservation-order-tracking-and-action-messaging.md)  
[Detalles de diseño: planificación de aprovisionamiento](design-details-supply-planning.md)   
[Procedimientos recomendados de configuración: planificación de suministros](setup-best-practices-supply-planning.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

