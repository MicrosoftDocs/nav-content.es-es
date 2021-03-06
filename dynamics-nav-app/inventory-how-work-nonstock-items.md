---
title: Crear y administrar los productos sin stock
description: "Describe cómo comercializar los productos no inventariables o los productos que no se mantienen en el inventario."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dd1497d0727935d4954f826eceb303761850dada
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-nonstock-items"></a>Procedimiento: Trabajar con productos sin stock
Puede ofrecer varios productos a sus clientes para su comodidad que no desea mantener en el inventario hasta que empiece a venderlos. Cuando desee empezar a mantener esos productos en el inventario, puede convertirlos en fichas de productos normales de dos formas.

* Desde una ficha de producto sin stock, cree una nueva ficha de producto basada en una plantilla.
* Desde una línea de pedido de ventas del tipo **Producto** con un campo **N.º* vacío, seleccione un producto sin stock. Se crea automáticamente una ficha de producto para el producto sin stock.

> [!NOTE]  
>   No puede seleccionar un producto sin stock de la ventana **Facturas venta**. Puede seleccionarlo desde la ventana **Oferta de ventas**, pero el producto sin stock no se convertirá en uno normal cuando utilice la función **Realizar pedido**.

Un producto sin stock normalmente tiene el número del proveedor que lo suministra. Para activar la conversión de una ficha de producto sin stock a una ficha normal, debe configurar cómo se convertirá la numeración del producto del vendedor a la suya.   

## <a name="to-create-a-nonstock-item"></a>Para crear productos sin stock
Las fichas de productos sin stock disponen de mucha menos información que las normales puesto que solo las utiliza en ofertas de ventas y en otras maneras. Por esa razón, se convertirán en fichas de producto normal antes de que pueda registrarles las transacciones de venta.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Para configurar cómo los números de productos sin stock se convierten en su numeración
Para activar la conversión de una ficha de producto sin stock en una ficha normal, primero debe configurar cómo se convertirá la numeración del producto del vendedor a su formato de número de producto.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Config. productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Para convertir un producto sin stock en un producto normal
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un producto sin stock que desee convertir a uno normal.
3. En la ventana **Ficha de producto sin stock**, seleccione la acción **Crear producto**.

Se ha creado una plantilla y una nueva ficha de producto con la información del producto sin stock rellenada previamente. Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Registrar nuevos productos](inventory-how-register-new-items.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Para vender un producto sin stock y convertirlo en un producto normal
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**. Rellene los campos de la ficha desplegable **General** para cada pedido. Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).
3. En una nueva línea de venta, en el campo **Tipo**, seleccione **Producto**, pero deje **N.º** campo vacío.
4. Elija la acción **Línea** y, a continuación, elija la acción **Seleccionar artículos sin stock**.

    El producto sin stock se ha convertido en un producto normal. Se ha creado una plantilla y una nueva ficha de producto con la información del producto sin stock rellenada previamente.
5. En la ventana **Productos sin stock**, seleccione el producto sin stock que desee vender y, a continuación, haga clic en **Aceptar**.
6. Cuando el pedido de venta ya está completo, seleccione la acción **Registrar**.

Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Registrar nuevos productos](inventory-how-register-new-items.md).

> [!NOTE]  
>   Un informe de referencia cruzada de un producto se crea automáticamente por el proveedor del producto entre el número del producto del proveedor y su nuevo número de producto.

## <a name="see-also"></a>Consulte también
[Registro de productos nuevos](inventory-how-register-new-items.md)  
[Cómo crear pedidos especiales](sales-how-to-create-special-orders.md)|  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

