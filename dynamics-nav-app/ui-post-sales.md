---
title: "Descripción de cómo registrar documentos de venta"
description: "Obtenga información sobre las diversas funciones de registro para registrar documentos de venta."
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7261e8faca0c14330e66093f8db3d44935c4d141
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="posting-sales"></a>Registrar ventas
En **Grupo contable** en un documento de ventas, puede elegir entre las funciones de registro siguientes:

* **Registrar**
* **Informe de prueba**
* **Registrar y enviar**
* **Registrar e imprimir**
* **Registrar y enviar por correo electrónico**
* **Registrar por lotes**
* **Vista previa de registro**

Una vez completadas todas las líneas e introducida toda la información en el pedido de venta, puede registrarlo. Esto crea un envío y una factura.

Cuando se registra un pedido de venta, se actualiza la cuenta del cliente, la contabilidad y los movimientos de producto.

Para cada pedido de venta, se crea un movimiento de venta en la tabla **Mov. contabilidad**. Se crea también un movimiento en la cuenta de cliente de la tabla **Mov. cliente** y un movimiento de contabilidad en la cuenta de cliente correspondiente. Además, el registro del pedido puede dar como resultado un movimiento de IVA y uno de contabilidad para el importe de descuento. El registro de un movimiento para el descuento depende del contenido del campo **Registro dto.** de la ventana **Conf. ventas y cobros**.

Por cada línea de pedido de venta, se creará un movimiento de producto en la tabla **Mov. producto** (si las líneas de venta contienen números de producto) o un movimiento de contabilidad en la tabla **Mov. contabilidad** (si las líneas de venta contienen una cuenta de contabilidad). Además, los pedidos de venta siempre se registran en las tablas **Histórico cab. albarán venta** y **Histórico cab. factura venta**.

> [!IMPORTANT]  
>   Cuando registre un pedido, puede crear un albarán de venta y una factura. Esto se puede realizar al mismo tiempo o de manera independiente. También puede crear un envío y una factura parciales completando los campos **Cantidad a enviar** y **Cantidad a facturar** en las líneas individuales del pedido de venta antes de registrar. Tenga en cuenta que no se puede crear una factura de algo que no se ha enviado. Es decir, para poder facturar, debe haber registrado un envío, o bien debe elegir enviar y facturar al mismo tiempo.

Una vez completado el registro, las líneas de venta registradas se quitan del pedido. Al terminar el registro aparece un mensaje de aviso. Después de esto, podrá ver los movimientos registrados en las diferentes ventanas que los contienen, como **Movs. cliente**, **Movs. contabilidad**, **Movs. producto**, **Histórico albaranes ventas** y **Histórico facturas venta**.

## <a name="see-also"></a>Consulte también
[Ventas](sales-manage-sales.md)  
[Enviar documentos por correo electrónico.](ui-how-send-documents-email.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


