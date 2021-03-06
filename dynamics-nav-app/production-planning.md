---
title: "Planificación de suministros"
description: "Preparar un plan ejecutable detallado y el programa de montaje final de producción para venta y la demanda de producción."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b904d539509c005f3d00b41a3724d1e70523059e
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="planning"></a>Planificación
Las operaciones de producción necesarias para transformar entradas en productos terminados se deben planificar a diario o semanalmente, en función del volumen y la naturaleza de los productos. [!INCLUDE[d365fin](includes/d365fin_md.md)] ofrece funciones para cubrir la demanda anticipada y real de las ventas, montaje y la producción, así como funciones de planificación de la distribución mediante unidades de almacenamiento y transferencias de ubicación.

> [!NOTE]
> En este tema se describe principalmente la planificación de empresas implicadas en la fabricación o gestión de ensamblaje donde los pedidos de suministro que se crean pueden ser tanto de producción, como de ensamblaje, transferencia o pedidos de compra. La interfaz principal de este trabajo de planificación es la ventana **Hoja planificación**.

> [!INCLUDE[d365fin](includes/d365fin_md.md)] también admite la planificación de suministro de las compañías mayoristas, en las que los pedidos de suministro que se creen solo pueden ser de transferencia y pedidos de compra. La interfaz principal de este trabajo de planificación es la ventana **Hoja de demanda**, que se describe indirectamente en este tema, pues la mayoría de las funciones de planificación se aplica a ambas hojas de trabajo.

Antes de planear y ejecutar órdenes de producción, debe configurar las capacidades de producción, como la creación de calendarios de planta, rutas y L.M. de producción y centros máquina. Para obtener más información, vea [Configurar fabricación](production-configure-production-processes.md).

La planificación puede considerarse como la preparación necesaria de pedidos de suministros en los departamentos de ensamblaje o de fabricación para cubrir la demanda. Si desea obtener más información, consulte [Gestión de ensamblaje](assembly-assemble-items.md) y [Fabricación](production-manage-manufacturing.md).

En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.   

|**Para**|**Vea**|  
|------------|-------------|  
|Obtenga una breve introducción de cómo se puede utilizar el sistema de planificación para detectar y priorizar la demanda y sugerir un plan de suministro consolidado.|[Sobre la funcionalidad de la planificación](production-about-planning-functionality.md)|
|Entienda cómo funcionan todos los aspectos del sistema de planificación y cómo ajustar los algoritmos para cumplir con los requisitos de planificación en distintos entornos.|[Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)|
|Aprender cómo la lógica de planificación diferencia entre la demanda en ubicaciones según la configuración UA y la demanda sin códigos de ubicación.|[Planificación con o sin almacenes](production-planning-with-without-locations.md)|
|Previsión de la demanda de producción presentada por ventas previstas y pedidos de producción.|[Creación de una previsión de producción](production-how-to-create-a-forecast.md)|  
|Crear órdenes de producción una a una automáticamente a partir del pedido de ventas, para cubrir la demanda exacta de la línea de pedido de ventas.|[Creación de órdenes de producción desde pedidos de venta](production-how-to-create-production-orders-from-sales-orders.md)|
|Crear una orden de producción de proyecto directamente desde un pedido de ventas multilínea que represente un proyecto de producción.|[Procedimiento: Planifique las órdenes de proyecto](production-how-to-plan-project-orders.md)|
|Utilizar la ventana **Programación de pedidos** para planificar manualmente para la demanda de ventas o producción un nivel L.MAT. de producción a la vez.|[Procedimiento: Planificar la nueva demanda de pedido por pedido](production-how-to-plan-for-new-demand.md)|
|Utilice la ventana **Hoja de planificación** para ejecutar las opciones de MPS y MRP para crear automáticamente alto nivel o planificación detallada en todos los niveles de producto.|[Cómo ejecutar la planificación completa, MPS o MRP](production-how-to-run-mps-and-mrp.md)|
|Ejecutar la hoja de demanda para crear automáticamente un plan de suministro detallado que cubra la demanda de artículos que sólo se reponen por compra o transferencia.|Página de **Hoja de demanda**|  
|Iniciar o actualizar una orden de producción como operaciones programadas a grosso modo en el programa de producción maestro.|[Cómo replanificar o actualizar órdenes de producción directamente](production-how-to-replan-refresh-production-orders.md)|
|Recalcular los calendarios de centro de trabajo o de máquina debido a cambios de planificación.|Sección “Para calcular un calendario de centro de trabajo” en [Procedimiento: Configurar los calendarios de planta](production-how-to-create-work-center-calendars.md)|
|Efectuar el seguimiento de la demanda de pedido (cantidad seguida), previsión, pedido de ventas abierto o parámetro de planificación (cantidad no seguida) que ha dado lugar a la línea de planificación en cuestión.|[Cómo hacer un seguimiento de las relaciones entre demanda y suministro](production-how-track-demand-supply.md)|
|Vea el inventario disponible proyectado de un producto con diferentes visualizaciones y vea qué necesidades brutas, recepciones de orden planificadas y otros influyen en él con el paso del tiempo.|[Consultar la disponibilidad de los productos](inventory-how-availability-overview.md)|  
|Realizar actividades de planificación seleccionadas, como modificar o agregar líneas de la hoja de planificación, en una visión gráfica del plan de suministros.|[Cómo modificar las sugerencias de planificación en una vista gráfica](production-how-to-modify-planning-suggestions-in-a-graphical-view.md)|

## <a name="see-also"></a>Consulte también
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Detalles de diseño: planificación de aprovisionamiento](design-details-supply-planning.md)   
[Procedimientos recomendados de configuración: planificación de suministros](setup-best-practices-supply-planning.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

