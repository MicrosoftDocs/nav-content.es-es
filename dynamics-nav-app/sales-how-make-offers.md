---
title: "Realización de ofertas"
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Realización de ofertas
Puede crear una oferta de venta para registrar la oferta a un cliente para vender determinados productos según términos de entrega y pago determinados. Puede enviar la oferta de venta al cliente para comunicar la oferta. Puede enviar por correo electrónico el documento como un documento PDF anexo. También puede rellenar previamente el cuerpo del correo electrónico con un resumen de la oferta. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).

Mientras negocia con el cliente, puede cambiar y reenviar la oferta de venta el número de veces necesario. Cuando el cliente acepta la oferta, convierte la oferta de venta a una factura de venta o un pedido de venta en el que se procesa la venta. Para obtener más información, consulte [Procedimiento: Facturar ventas](sales-how-invoice-sales.md) o [Procedimiento: Vender productos](sales-how-sell-products.md).

Los productos pueden ser productos de inventario y servicios. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md). El proceso de la oferta de venta es el mismo para ambos tipos de producto.

**Nota**: En Dynamics NAV, se usa el término “producto” para denominar los artículos.

Puede rellenar los campos de clientes en la oferta de venta de dos formas en función de si el cliente ya está registrado.

## <a name="to-create-a-sales-quote"></a>Para crear una oferta de venta
1. En la página Inicio, seleccione la acción **Oferta de venta**.  
2. En el campo **Cliente**, escriba el nombre de un cliente existente.

    Otros campos de la ventana **Oferta de venta** se rellenarán con la información estándar del cliente seleccionado. Si el cliente no está registrado, realice los pasos siguientes:

3. En el campo **Cliente**, escriba el nombre del cliente nuevo.
4. En el cuadro de diálogo de registro de nuevos clientes, haga clic en el botón **Sí**.
5. En la ventana **Seleccionar una plantilla para un cliente nuevo**, seleccione una plantilla en la que se basará la nueva ficha de cliente y, a continuación, haga clic en el botón **Aceptar**.
6. Una nueva ficha de cliente se abre, prellenada con información sobre la plantilla de cliente seleccionada. El campo **Nombre** se rellena con el nombre del nuevo cliente que especificó en la factura de venta.
7. Rellene los campos restantes de la ficha de cliente. Para obtener más información, vea [Procedimiento: Registrar nuevos clientes](sales-how-register-new-customers.md).  
8. Cuando haya finalizado la ficha de cliente, haga clic en el botón **Aceptar** para volver a la ventana **Oferta de venta**.

    Muchos campos de la oferta de venta se rellenan con la información especificada en la nueva ficha de cliente.
9. Rellene los campos en la ventana **Oferta de venta** según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

    Ya está preparado para rellenar las líneas de la oferta de venta con los productos de inventario o los servicios que quiera ofrecer al cliente.

    **Nota**: Si ha configurado líneas de venta periódicas para el cliente, como un pedido de reabastecimiento mensual, puede insertar estas líneas en la oferta seleccionando la acción **Obtener líneas de venta periódicas**.
10. En la ficha desplegable **Líneas**, en el campo **N.º producto**,  introduzca el número de un producto de inventario o servicio.
11. En el campo **Cantidad**, escriba el número de productos que se van a ofrecer.

    **Nota**: Para los producto de tipo Servicio la cantidad es una unidad de tiempo, por ejemplo horas, según se indica en el campo **Cód. unidad medida** en la línea.

    El campo **Importe línea** se actualiza para mostrar el valor del campo **Precio venta** multiplicado por el valor del campo **Cantidad**.

    El precio y el importe de las líneas se muestran con o sin IVA dependiendo de qué seleccione en el campo **Precios incluyendo el impuesto de ventas** en la ficha del cliente.
12. En el campo **% Descuento línea**, especifique un porcentaje si desea conceder al cliente un descuento para el producto. El valor del campo **Importe de línea** se actualiza según corresponde.

    **Nota**: Si ha configurado precios de producto especiales en la ficha desplegable **Precios venta y descuentos línea ventas** en la ficha del producto o en la del cliente, el porcentaje de descuento, el precio y el importe de línea en la línea de la oferta se actualizan automáticamente si se cumplen los criterios acordados para el precio. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).
13. Para agregar un comentario acerca de la línea de oferta que el cliente puede ver en la oferta de venta impresa, escriba un texto en el campo **Descripción** en una línea vacía.  
14. Repita los pasos 10 a 13 para cada producto que desee ofertar al cliente.

    Los totales por debajo de las líneas se calculan automáticamente cuando se crean o modifican las líneas.
15. En el campo **Importe descuento factura**, especifique un importe que se debe descontar del valor que aparece en el campo **Total impuesto incl.** en la parte inferior de la factura.

    **Nota**: Si ha configurado descuentos en factura para el cliente, el valor porcentual especificado se inserta automáticamente en el campo **% descuento en factura** si se cumplen los criterios, y el importe relacionado se inserta en el campo **Descuento en factura excluyendo IVA**. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).
16. Cuando las líneas de la oferta de venta ya estén completas, seleccione la acción **Enviar por correo electrónico** o **Imprimir**.

    Si ha seleccionado la acción **Enviar por correo electrónico**, se adjunta automáticamente un archivo PDF a un mensaje correo electrónico para el cliente. Puede configurar el correo electrónico para que contenga un resumen de la oferta. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).
17. Si el cliente acepta la oferta, seleccione la acción **Generar factura** o **Realizar pedido**.

La oferta de venta se quita de la base de datos. Una factura de venta o un pedido de venta se crea a partir de la información en la oferta de venta en la que puede procesar la venta. En el campo **N.º oferta**, de la factura de venta o del pedido de venta puede ver el número de la oferta de venta a partir de la que se creó. Para obtener más información, consulte [Procedimiento: Facturar ventas](sales-how-invoice-sales.md) o [Procedimiento: Vender productos](sales-how-sell-products.md).

## <a name="see-also"></a>Consulte también  
[Gestionar ventas](sales-manage-sales.md)  
[Configurar ventas](sales-setup-sales.md)  
[Enviar documentos por correo electrónico.](ui-how-send-documents-email.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

