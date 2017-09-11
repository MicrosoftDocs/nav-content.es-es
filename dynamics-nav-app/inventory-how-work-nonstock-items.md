---
title: 'Procedimiento: Trabajar con productos sin stock'
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 6d99e06c167d3b86db97883c02c8bf5cd746ae10
ms.contentlocale: es-es
ms.lasthandoff: 07/19/2017

---

# Procedimiento: Trabajar con productos sin stock
Puede ofrecer varios productos a sus clientes para su comodidad que no desea mantener en el inventario hasta que empiece a venderlos. Cuando desee empezar a mantener esos productos en el inventario, puede convertirlos en fichas de productos normales de dos formas.

- Desde una ficha de producto sin stock, cree una nueva ficha de producto basada en una plantilla.
- Desde una línea de pedido de ventas que tenga el campo **Producto** vacío, seleccione un producto sin stock. Cuando registra la venta, se crea automáticamente una ficha de producto para el producto sin stock.

**Nota**: No puede seleccionar un producto sin stock de la ventana **Facturas venta**. Puede seleccionarlo desde la ventana **Oferta de ventas**, pero el producto sin stock no se convertirá en uno normal cuando utilice la función **Realizar pedido**.

Un producto sin stock normalmente tiene el número del proveedor que lo suministra. Para activar la conversión de una ficha de producto sin stock a una ficha normal, debe configurar cómo se convertirá la numeración del producto del vendedor a la suya.   

## Para crear productos sin stock
Las fichas de productos sin stock disponen de mucha menos información que las normales puesto que solo las utiliza en ofertas de ventas y en otras maneras. Por esa razón, se convertirán en fichas de producto normal antes de que pueda registrarles las transacciones de venta.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

## Para configurar cómo los números de productos sin stock se convierten en su numeración  
Para activar la conversión de una ficha de producto sin stock en una ficha normal, primero debe configurar cómo se convertirá la numeración del producto del vendedor a su formato de número de producto.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.

## Para convertir un producto sin stock en un producto normal
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos sin stock** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un producto sin stock que desee convertir a uno normal.
3. En la ventana **Ficha de producto sin stock**, seleccione la acción **Crear producto**.

Se ha creado una plantilla y una nueva ficha de producto con la información del producto sin stock rellenada previamente. Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

## Para vender un producto sin stock y convertirlo en un producto normal
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Pedidos de ventas** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**. rellene los campos de la ficha desplegable **General** para cada pedido.
3. En una nueva línea de pedido, deje el campo **Producto** vacío, seleccione **Línea**, **Funciones** y, a continuación, **Productos sin stock**.

    El producto sin stock se ha convertido en un producto normal. Se ha creado una plantilla y una nueva ficha de producto con la información del producto sin stock rellenada previamente.
4. En la ventana **Productos sin stock**, seleccione el producto sin stock que desee vender y, a continuación, haga clic en **Aceptar**.
5. Cuando el pedido de venta ya está completo, seleccione la acción **Registrar**.

Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

**Nota**: Un informe de referencia cruzada de un producto se crea automáticamente por el proveedor del producto entre el número del producto del proveedor y su nuevo número de producto.

## Consulte también
[Registro de productos nuevos](inventory-how-register-new-products.md)  
[Gestionar inventario](inventory-manage-inventory.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

