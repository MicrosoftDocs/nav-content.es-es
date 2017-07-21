---
title: "Procedimiento: Realizar envíos directos"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Procedimiento: Realizar envíos directos
Un envío directo es el envío de los productos de uno de sus proveedores directamente a uno de sus clientes.

Cuando marca un pedido de venta con el envío directo y crea un pedido especificando el cliente en el campo **Venta a-N.º cliente** puede vincular los dos documentos y así asignar instrucciones al proveedor para que envíe el producto directamente al cliente.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Para crear un pedido de venta de envío directo
Para preparar un envío directo cree un pedido de venta como si fuese normal, pero indique en la línea de ventas que dicha venta requiere un envío directo.

1. Cree un pedido de ventas para un artículo. Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).
2. En la línea del pedido de venta del artículo con envío directo, seleccione la casilla **Envío directo**.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Para crear pedidos de compra para envíos directos
Para preparar un envío directo de un producto que se va a vender, cree un pedido de compra como si fuese normal, pero indique en el pedido que el producto debe enviarse directamente al cliente no a usted.

1. Cree un pedido de compra. No rellene ningún campo en las líneas. Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).
2. En el campo **Venta a-N.º cliente**, seleccione el cliente al que le está vendiendo.
3. Elija la acción **Envíos directos** y, a continuación, **Traer pedido venta**.
4. En la ventana **Lista ventas**, seleccione el pedido de ventas que ha preparado en la sección "Para crear un pedido de venta de envío directo".
5. Elija el botón **Aceptar**.

La información de la línea del pedido de venta se inserta en las líneas del pedido de compra.

Ahora puede asignar instrucciones al proveedor para que envíe los productos al cliente, por ejemplo, enviando el pedido de compra por correo electrónico en formato PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Para ver el pedido de compra vinculado al pedido de venta.
1. Seleccione la línea del envío directo del pedido de compra, elija las acciones **Pedido**, **Envío directo** y, a continuación, **Pedido de compra**.

El pedido de compra vinculado se abre.

## <a name="to-post-a-drop-shipment"></a>Para registrar un envío directo
Cuando el proveedor ha enviado los artículos, puede establecer los pedidos de venta como enviados. También puede registrar el pedido de compra, pero solo con la opción **Recibir** hasta que se haya facturado el pedido de ventas.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Pedidos de ventas** y, a continuación, seleccione el vínculo relacionado.
2. Abra el pedido de venta que ha creado en la sección "Para crear un pedido de venta de envío directo".
3. En el campo **Cantidad a enviar**, especifiqué qué cantidad del pedido debe enviarse, todo o solo una parte.
3. Seleccione la acción **Registrar** o **Registrar y enviar**.
4. Elija la opción **Enviar** para facturar más adelante o la opción **Enviar y facturar** para facturar ahora.

## <a name="see-also"></a>Consulte también
[Vender productos](sales-how-sell-products.md)    
[Registro de compras](purchasing-how-record-purchases.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar inventario](inventory-manage-inventory.md)      
[Trabajar con Dynamics NAV](ui-work-product.md)

