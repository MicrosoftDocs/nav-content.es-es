---
title: Procesamiento de devoluciones de ventas o cancelaciones
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Procesamiento de devoluciones de ventas o cancelaciones
Si el cliente desea devolver u obtener un reembolso de algún producto o servicio que usted ha vendido y que le han pagado, debe crear y registrar una abono de ventas que especifique el cambio requerido. Para incluir la información correcta de la factura de venta, puede crear el abono de venta de la factura de venta registrada o usar una función de copia.

Además de la original factura de venta registrada, puede liquidar el abono de venta a otros documentos de venta, por ejemplo otra factura de venta registrada, porque el cliente también devuelve los productos entregados con dicha factura.

Una devolución o reembolso se puede relacionar con solo algunos de los productos o servicios de la factura de venta original. En ese caso, debe editar la información de las líneas del abono de venta. Cuando se registra el abono de venta, se revierten los documentos de venta que se ven afectados por el cambio y se puede crear un pago de devolución para el cliente.

Puede enviar el abono de venta registrado al cliente para confirmar la devolución o cancelación y comunicar que el valor relacionado se reembolsará, por ejemplo, cuando se devuelven los productos.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Para crear un nuevo abono de venta desde una factura de venta registrada.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de ventas registradas** y, a continuación, elija el enlace relacionado.  
2. En la ventana **Facturas de venta registradas**, seleccione la factura de ventas que desea revertir y, a continuación, seleccione la acción **Crear abono correctivo**.

    La mayoría de los campos de la cabecera de abono de venta se rellenan con la información de la factura de ventas registrada. Puede modificar todos los campos, por ejemplo, mediante la nueva información que indica el contrato de devolución.
3. Edite la información de las líneas según el contrato, como por ejemplo el número de productos devueltos o el importe que se reembolsará.
4. Seleccione la acción **Liquidar movs.**.
5. En la ventana **Liquidar movimientos cliente**, seleccione la línea con el documento de ventas registrado al que desee liquidar el abono de ventas y, a continuación, seleccione la acción **Liq. por id.**.

    El número del abono de ventas se inserta en el campo **Liq. por id**.  
6. En la línea del campo **Importe a liquidar**, introduzca el importe que desea liquidar si es menor que el importe original.

    En la parte inferior de la ventana **Liq. movs. cliente**, puede observar el importe total a liquidar para revertir todos los movimientos correspondientes, concretamente cuando el valor en el campo **Balanza** es cero.  
7. Elija el botón **Aceptar**. Cuando registra el abono de venta, este se aplicará a los documentos de venta registrados especificados.

    Cuando ha creado o editado las líneas de abono de venta necesarias y se han especificado una o varias aplicaciones, puede empezar a registrar el abono de venta.
8. Seleccione la acción **Registrar y enviar**.

El cuadro de diálogo de **Registrar y enviar confirmación** se abre para mostrar el método de envío preferido para el cliente. Puede cambiar el método de envío seleccionando el botón de búsqueda en el campo **Enviar documento a**. Para obtener más información, vea [Procedimiento: Configurar los perfiles de envío de documentos](sales-how-setup-document-send-profiles.md).

Los documentos de venta registrados a los que ha aplicado el abono están invertidas y se puede crear un pago del reembolso para el cliente. El abono de venta se ha eliminado y remplazado por un nuevo documento de la lista de abonos de venta registrados.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Para crear un abono de ventas desde cero
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de ventas registradas** y, a continuación, elija el enlace relacionado.
2. Seleccione la acción **Nuevo** para abrir un abono de ventas vacío.
3. En el campo **Cliente**, escriba el nombre de un cliente existente.
4. Elija la acción **Copiar documento**.
5. En la ventana **Copiar documento de ventas**, en el campo **Tipo de documento**, seleccione el campo **Factura registrada**
6. Seleccione el **N.º documento**. para abrir la ventana **Facturas de venta registradas** y, a continuación, seleccione la factura de ventas registrada que contiene las líneas que desea revertir.
7. Seleccione la casilla **Recalcular líneas** si desea que las líneas de factura de venta registradas copiadas se actualicen con los cambios en el precio y el coste unitario del producto desde que la factura fue registrada.
8. Elija el botón **Aceptar**. Las líneas de factura copiadas se insertarán en el abono de venta.
9. Complete el abono de venta como se explica en la sección "Para crear un abono de ventas de una factura de ventas registrada" en este tema.

## <a name="see-also"></a>Consulte también  
[Gestionar ventas](sales-manage-sales.md)  
[Configurar ventas](sales-setup-sales.md)  
[Enviar documentos por correo electrónico.](ui-how-send-documents-email.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

