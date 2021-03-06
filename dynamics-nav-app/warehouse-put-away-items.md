---
title: Ubicar productos
description: "La actividad de almacén consistente en ubicar los productos una vez éstos se reciben o elaboran se realiza de modo distinto según estén configuradas las funciones de gestión del almacén."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0b68ef1b4c73eef1ac82d59587011a0fcdead096
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="putting-items-away"></a>Configurando los artículos componentes
La actividad de almacén consistente en ubicar los productos una vez éstos se reciben o elaboran se realiza de modo distinto según estén configuradas las funciones de gestión del almacén. La complejidad puede oscilar desde la ausencia total de funciones de almacén, pasando por configuraciones básicas de almacén para la gestión pedido por pedido en sólo una o más actividades, hasta configuraciones más avanzadas en las que todas las actividades del almacén se llevan a cabo como parte de un flujo de trabajo dirigido. Para obtener más información, consulte [Configuración de la administración de almacén](warehouse-setup-warehouse.md).

Si decide que desea organizar y registrar su información de ubicación con documentos del almacén, active el campo **Ubicación requerida** en la ficha de almacén. Esto indica que cuando tenga que dar entrada a productos en el almacén mediante un documento de origen de entrada, desea que la ubicación de estos productos se controle mediante el sistema. Un documento de origen de entrada puede ser un pedido de compra, una devolución de ventas, un pedido de transferencia de salida o una orden de producción cuya salida está preparados para ubicarse.  

Si el almacén está configurado para utilizar el proceso de ubicación, pero no el proceso de recepción, utilice la ventana **Ubicac. inventario** para organizar la información de ubicación, imprimirla, especificar el resultado de la ubicación real y registrar la información de ubicación, que, a su vez, registra la información de recepción del documento de origen. En el caso de un pedido de producción, se registra la salida del pedido y se finaliza el pedido de producción.

Si el almacén está configurado para requerir los procesos de ubicación y recepción, con lo que ha activado los campos **Recepción requerida** y **Ubicación requerida** en la ficha de almacén, existe un proceso diferente para ubicar productos. En este caso, utilizará la ventana **Ubicar almacén** para gestionar la ubicación. Ubicar almacén funciona de forma similar a la ubicación de inventario, excepto que en vez de registrar la información, se registra la ubicación. Observe que el registro de ubicación de almacén no registra la recepción de los artículos. Simplemente actualiza el contenido de la ubicación. Como administrador del almacén, puede utilizar las hojas de trabajo de ubicación para organizar la información antes de crear las instrucciones individuales de ubicación de almacén.

En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.   

|**Para**|**Vea**|  
|------------|-------------|  
|Registre el recibo de productos directamente desde el documento de órdenes de entrada y registre la ubicación, ya que no existe ninguna configuración de almacén.|[Cómo recibir productos](warehouse-how-receive-items.md)|  
|Ubicar los productos pedido a pedido y registrar la recepción como parte de la misma actividad, en una configuración básica de almacén.|[Ubicación de productos con ubicación de inventario](warehouse-how-to-put-items-away-with-inventory-put-aways.md)|  
|Ubicar productos de distintos pedidos en una configuración avanzada de almacén.|[Procedimiento: ubique productos con ubicaciones de inventario](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)|  
|Ubicar productos producidos o ensamblados en una configuración básica o avanzada de inventario.|[Cómo ubicar la salida de producción o la salida de ensamblado](warehouse-how-to-put-away-production-output.md)|
|Planificar instrucciones optimizadas de ubicación para un número de recepciones de almacén registradas en lugar de tener empleados del almacén actuando directamente en las recepciones.|[Procedimiento: planifique ubicaciones en hojas de trabajo](warehouse-how-to-plan-put-aways-in-worksheets.md)|  
|Recolocar los productos cuyo picking técnico se realizó en una fase interna de picking, por ejemplo para una orden de producción que no consumió la cantidad prevista.|[Realizar el picking y la ubicación sin un documento de origen](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Dividir una línea de ubicación para color parte de la cantidad a ubicar en ubicaciones disponibles puesto que la ubicación designada se encuentra llena.|[Procedimiento: divida las líneas de actividad de almacén](warehouse-how-to-split-warehouse-activity-lines.md)|
|Obtener acceso inmediato a las ubicaciones asignadas al usuario en calidad de empleado del almacén.|[Procedimiento: busque las asignaciones de almacén](warehouse-how-to-find-your-warehouse-assignments.md)|    

## <a name="see-also"></a>Consulte también  
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

