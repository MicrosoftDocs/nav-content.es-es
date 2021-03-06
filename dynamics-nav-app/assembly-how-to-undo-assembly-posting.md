---
title: Deshacer registro de ensamblado
description: Puede que, a veces, tenga que deshacer un pedido de ensamblado registrado, por ejemplo cuando se haya registrado con errores que deban corregirse, o porque no deban haberse registrado en el primer lugar y deban revertirse.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3ba93dd182aa1591f5d24398d4b749942d38bb4b
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-undo-assembly-posting"></a>Procedimiento: deshacer registro de ensamblado
Puede que, a veces, tenga que deshacer un pedido de ensamblado registrado, por ejemplo cuando se haya registrado con errores que deban corregirse, o porque no deban haberse registrado en el primer lugar y deban revertirse.

Cuando se deshace un pedido de ensamblado registrado, se crea un grupo de los movimientos de producto correctores para revertir las entradas originales. Cada entrada positiva de salida para el artículo de montaje se revierte mediante una entrada negativa de salida. Cada entrada de consumo negativo de un componente de ensamblado se revierte mediante una entrada de consumo positivo. La solicitud del coste fijo se crea automáticamente entre las entradas correctoras y originales para garantizar una reversión exacta del coste.  

Cuando se deshace totalmente un pedido de ensamblado registrado, puede elegir volver a crear el pedido de ensamblado en su estado original, por ejemplo para hacer las correcciones antes de volver a registrarlo. También puede decidir no volver a crearlo.  

Cuando se deshace parcialmente un pedido de ensamblado registrado, todos los campos de cantidad afectados, por ejemplo **Cantidad ensamblada**, **Cantidad consumida** y **Cantidad pendiente**, se restablecen a los valores que tenían antes del registro en cuestión.  

Para volver a crear o restaurar los pedidos de ensamblado, debe aplicar las condiciones siguientes al artículo de montaje que se produjo en el registro original:  

-   Debe aún estar en el inventario, es decir, no debe haberse vendido ni consumido de otra forma por las transacciones de salida.  
-   No debe estar reservado.  
-   Debe existir en la ubicación que de salida.  

Además, los pedidos de ensamblado existentes se pueden restablecer sólo si no se modifican el número y la secuencia de líneas en el pedido de ensamblado original.  

> [!TIP]  
>  Para solucionar conflictos debido a variaciones de línea, puede revertir manualmente los cambios en las líneas en cuestión antes de deshacer el pedido de ensamblado registrado relacionado. También puede registrar el pedido de ensamblado totalmente y, después, seleccionarlo para reconstruirlo al deshacer el registro.  

El procedimiento siguiente describe cómo deshacer los pedidos de ensamblado registrado donde los artículos se ensamblaron para stock. Si desea deshacer los pedidos de ensamblado registrado donde los artículos se ensamblaron para pedido de venta, deberá usar la función **Deshacer envío** en el envío registrado relacionado con el pedido de ensamblado registrado. Para obtener más información, consulte [Revertir registros](finance-how-reverse-journal-posting.md). Deshacer el pedido de ensamblado registrado se produce entonces automáticamente tal como que se describe en este tema.  

## <a name="to-undo-posting-of-an-assembly-order"></a>Para deshacer el registro de un pedido de ensamblado  
1.  Para deshacer total o parcialmente el pedido de ensamblado registrado, seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de ensamblado registrados** y seleccione el enlace relacionado.  

    Se abrirá la ventana **Pedidos de ensamblado registrados** y mostrará uno o más pedidos de ensamblado registrado que se registren del pedido de ensamblado en cuestión. Cada registro parcial crea un pedido de ensamblado registrado diferente.  
2.  Abra el pedido de ensamblado registrado que desea revertir y elija la acción **Deshacer ensamblado**.  

    Si el pedido de ensamblado registrado que desea deshacer está relacionado con uno totalmente registrado que se ha eliminado, tiene la opción de reconstruirlo, normalmente porque desea volver a procesarlo.  
3.  Si desea volver a crear el pedido de ensamblado, seleccione el botón de **Sí**. Para deshacer el registro sin la reconstrucción del pedido de ensamblado relacionado, seleccione el botón **No**.  

El campo **Revertido** de la cabecera del pedido de ensamblado cambia a **Sí**. El registro de pedido de ensamblado ahora se revierte, y puede empezar a procesar el pedido de ensamblado completo si elige lo volver a crear o el pedido de ensamblado abierto que ha restablecido a su estado original.  

> [!NOTE]  
>  Para restaurar las cantidades de los registros parciales múltiples en un pedido de ensamblado, deberá deshacer todos los pedidos de ensamblado registrados en cuestión siguiendo los pasos 1 a 3 anterior para cada pedido de ensamblado registrado.  

## <a name="see-also"></a>Consulte también  
[Gestión de ensamblaje](assembly-assemble-items.md)  
[Revertir registros](finance-how-reverse-journal-posting.md)  
[Procesamiento de devoluciones de ventas o cancelaciones](sales-how-process-sales-returns-cancellations.md)    
[Trabajar con listas de materiales](inventory-how-work-BOMs.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

