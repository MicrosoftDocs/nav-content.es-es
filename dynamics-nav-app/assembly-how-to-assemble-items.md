---
title: Ensamble productos
description: "Si el campo **Sistema reposición** en la ficha del artículo contiene **Montaje**, el método predeterminado para suministrar el artículo será ensamblarlo desde los componentes definidos y potencialmente por un recurso definido."
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
ms.openlocfilehash: b7f371c48aa70d2b99ce7b7333b92a63d7764f28
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-assemble-items"></a>Procedimiento: ensamble productos
Si el campo **Sistema reposición** en la ficha del artículo contiene **Montaje**, el método predeterminado para suministrar el artículo será ensamblarlo desde los componentes definidos y potencialmente por un recurso definido.  

Los componentes y los recursos que forman esta clase de artículo de ensamblado deben definirse en un L.M. de ensamblado. Para obtener más información, consulte [Procedimiento: Trabajar con listas de materiales](inventory-how-work-BOMs.md).  

Los artículos de ensamblado se pueden configurar para dos procesos de ensamblado diferentes:  

-   Ensamblar para stock.  
-   Ensamblar para pedido  

Se utiliza normalmente **Ensamblar para stock** para los artículos que se desea ensamblar antes de la venta, como para prepararse para una campaña de equipo, y mantenerlo en stock hasta que se soliciten. Estos artículos suelen ser estándar, como equipos embalados que no ofrecen personalización según las solicitudes de cliente.  

Utilice normalmente **Ensamblar para pedido** para los artículos que no desee almacenar porque espera personalizarlos según lo solicitado por el cliente o porque desee minimizar el coste que conlleva el inventario suministrándolo en el momento oportuno. Para obtener más información, consulte [Procedimiento: Venta de artículos ensamblados para pedido](assembly-how-to-sell-items-assembled-to-order.md).  

Para obtener más información acerca de cómo configurar un elemento del ensamblado, consulte [Comprender Ensamblar para pedido y Ensamblar para stock](assembly-assemble-to-order-or-assemble-to-stock.md).  

Estas opciones de configuración son los valores predeterminados para controlar cómo se procesan inicialmente las líneas de ventas y de pedido de ensamblado. Puede iniciar a partir de estos valores predeterminados y suministrar el artículo de ensamblado de la forma más óptima al procesar una venta. Para obtener más información, consulte [Procedimiento: Venta de productos de inventario en los flujos de ensamblar para pedido](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md) y [Procedimiento: Venta de productos de ensamblado para pedido y productos de inventario juntos](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).

> [!NOTE]  
> Los componentes de ensamblaje se manejan de forma especial en configuraciones básicas de almacén. Para obtener más información, vea la sección “Tratamiento de productos ensamblar para pedido en los picking de inventario” en [Cómo realizar picking de productos con picking inventario](warehouse-how-to-pick-items-with-inventory-picks.md).   

En este procedimiento se crea y procesa un pedido de ensamblado para los artículos que se ensamblan para stock, lo que significa que no tiene un pedido de venta vinculado. Los pasos incluyen la iniciación del pedido de ensamblado, gestionando los problemas potenciales de disponibilidad de componente y registrando parcialmente la salida del artículo de montaje.

## <a name="to-assemble-an-item"></a>Para ensamblar un artículo  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de ensamblados** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**. Se abrirá la ventana **Nuevo pedido de ensamblado**.  
3.  Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  En el campo **Nº producto**, introduzca el número del producto que desea solicitar. El campo se filtra para mostrar solo los artículos configurados para el ensamblado, lo que significa que tienen asignado el ensamblado L.M..  
5.  En el campo **Cantidad**, especifique cuántas unidades del artículo desea que se ensamblen.  

    > [!NOTE]  
    >  Si uno o más componentes no están disponibles para cubrir la cantidad introducida del artículo de montaje en la fecha de vencimiento determinada, la ventana **Disponibilidad de ensamblado** se abrirá automáticamente para proporcionar información detallada acerca de cuántos productos de ensamblado se pueden ensamblar basándose en la disponibilidad de componentes. Para obtener más información, consulte [Consultar la disponibilidad de los productos](inventory-how-availability-overview.md).  Cuando se cierra la ventana, el pedido de ensamblado se crea con las alertas de la disponibilidad de las líneas de componente afectados.  

    Las líneas del pedido de ensamblado se rellenan automáticamente con el contenido del L.M. de ensamblado y con las cantidades de línea según la cabecera del pedido de ensamblado.  

    > [!NOTE]  
    >  Si la ventana **Disponibilidad de ensamblado** se abre cuando se rellena la cabecera del pedido de ensamblado, cada línea asignado de pedido de ensamblado afectada contiene **Sí** en el campo **Advertencia disp.** con un vínculo a la información detallada de disponibilidad. Para obtener más información, consulte Comprobar disponibilidad. Puede resolver un problema de disponibilidad de componente posponiendo la fecha inicial, reemplazando al componente por otro artículo o seleccionando un sustituto disponible si hay alguno definido.  

6.  En el campo **Cantidad a ensamblar**, introduzca cuántas unidades del artículo de ensamblado va a registrar como salida la próxima vez que registre el pedido de ensamblado. Esta cantidad puede ser menor que el valor del campo **Cantidad** para reflejar un registro parcial de salida.  

    > [!NOTE]  
    >  Para garantizar que el registro de consumo del componente cumpla el registro de salida del artículo de ensamblado, los campos de cantidad en las líneas del pedido de ensamblado ajustan automáticamente el valor que se introduce en el campo **Cantidad a ensamblar**.  
7.  En líneas de pedido de ensamblado de tipo **Producto** o **Recurso**, en el campo **Cantidad para consumir**, introduzca cuántas unidades va a registrar como consumidas la próxima vez que registre el pedido de ensamblado. De forma predeterminada, se insertan la cantidad esperada para consumir según el L.M. de ensamblado y la cantidad de la cabecera del pedido de ensamblado, pero puede aumentarla o disminuirla, como para reflejar un exceso de consumo de los componentes o que se han utilizado recursos adicionales.  
8.  Cuando esté listo listas para realizar el registro parcial o completamente, elija la acción **Registrar**.  

    > [!NOTE]  
    >  Si las advertencias todavía están presentes en algunas de las líneas del pedido de ensamblado, se bloquea el registro. Se muestra un mensaje sobre que el o los componentes no están en inventario.  

Después de que el registrar se realice correctamente, el artículo de ensamblado se registra como salida al código de almacén y al potencial código de ubicación definidos en el pedido de ensamblado. Para los pedidos de ensamblado creados manualmente, la ubicación se puede copiar desde el campo de instalación **Ubicación pred. pedidos**. Para los flujos de ensamblar para pedido, el código de almacén se copia de la línea del pedido de venta.  

## <a name="see-also"></a>Consulte también
[Gestión de ensamblaje](assembly-assemble-items.md)  
[Trabajar con listas de materiales](inventory-how-work-BOMs.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

