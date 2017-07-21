---
title: Registrar compras
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c03d031e951bc185b18bedaf428d414c1fe2e7d1
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="posting-purchases"></a>Registrar compras
En **Grupo contable** en un documento de compra, puede elegir entre las funciones de registro siguientes:

- **Registrar**
- **Vista previa de registro**
- **Registrar e imprimir**
- **Informe de prueba**
- **Registrar por lotes**

Una vez completadas todas las líneas e introducida la información en el pedido de compra, podrá registrarlo; es decir, crear un albarán de compra y una factura.

Cuando se registra un pedido de compra, se actualiza la cuenta del proveedor, la contabilidad y los movimientos de producto.

Por cada pedido de compra, se crea un movimiento de compra en la tabla **Mov. contabilidad**. Se crea también un movimiento en la cuenta de proveedor de la tabla **Mov. proveedor** y un movimiento de contabilidad en la correspondiente cuenta de pagos. Además, el registro del pedido puede dar como resultado un movimiento de IVA y uno de contabilidad para el importe de descuento. El que se registre un movimiento para el descuento depende del contenido del campo **Registro dto.** de la ventana **Conf. compras y pagos**.

Por cada línea de pedido de compra, se creará un movimiento de producto en la tabla **Mov. producto** (si las líneas de compra contienen números de producto) o un movimiento de contabilidad en la tabla **Mov. contabilidad** (si las líneas de compra contienen una cuenta de contabilidad). Además, los pedidos de compra siempre se registran en las tablas **Histórico cab. albarán compra** e **Histórico cab. factura compra**.

Antes de comenzar a registrar, podrá imprimir un informe que contenga toda la información del pedido de compra y que indique cualquier error que pueda existir allí. Para imprimir este informe, elija **Registro** y, a continuación, **Informe de prueba**.

**Importante**: Cuando registre un pedido, podrá crear tanto un albarán de compra como una factura. Esto se puede hacer simultánea o independientemente. También puede crear una recepción y una factura parciales completando los campos **Cantidad a recibir** o **Cantidad a facturar** en las líneas individuales del pedido de compra antes de registrar. Tenga en cuenta que no puede crear una factura de algo no se ha recibido. Es decir, antes de poder facturar debe haber registrado un albarán de compra o haber elegido recibir y facturar al mismo tiempo.

Puede registrar o registrar e imprimir. Si elije registrar e imprimir, un informe se imprime cuando se registre el pedido. También puede elegir la función **Registrar por lotes**, que permite registrar varios pedidos a la vez.

Una vez finalizado el registro, las líneas de compra registradas se quitan del pedido. Al terminar el registro aparece un mensaje de aviso. Después de esto, podrá ver los movimientos registrados en las diferentes ventanas que los contienen, como **Movs. proveedores**, **Movs, contabilidad**, **Movs. productos**, **Albaranes compra** y **Histórico facturas compra**.

## <a name="see-also"></a>Consulte también
[Registrar documentos y diarios](ui-post-documents-journals.md)

