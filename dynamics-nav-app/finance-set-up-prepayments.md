---
title: Configurar prepagos
description: "Los prepagos son pagos que se facturan y registran en un pedido de prepago de ventas o compras antes de la facturación final. Puede requerir un depósito antes de fabricar productos bajo pedido o puede requerir el pago antes de enviar productos a un cliente. La funcionalidad de prepagos le permite facturar y cobrar depósitos requeridos de los clientes o remitir depósitos a proveedores. De este modo, puede asegurar que todos los pagos se registran contra una factura."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cdbd9113d43aaab48788e18e7b56cb7d8eef5410
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-prepayments"></a>Definir prepagos
Si desea que sus clientes realicen el pago antes de enviarles un pedido o su proveedor le requiere que efectúe el pago antes de enviarle un pedido, puede utilizar la funcionalidad Prepago. La funcionalidad le permite facturar y cobrar depósitos requeridos de los clientes o remitir depósitos a proveedores y asegurarse de que todos los pagos parciales se contabilicen con una factura. Para obtener más información, consulte [Crear una factura de prepago](finance-how-to-create-prepayment-invoices.md).

Para poder registrar facturas de prepago, debe configurar las cuentas auxiliares en la contabilidad y configurar series numéricas para documentos de prepago.  

Puede definir el porcentaje del importe de línea que se va a facturar para el prepago, para un cliente o proveedor, para todos los productos o para algunos. Una vez que finalice la configuración, puede generar facturas de prepago a partir de pedidos de compra y venta. Puede usar los porcentajes predeterminados para cada línea de compra o venta o cambiar los importes en la factura según sea necesario. Por ejemplo, puede especificar un importe total para todo el pedido.  

Dado que el importe de prepago pertenece al comprador hasta que haya recibido los productos o los servicios, debe definir las cuentas de contabilidad para que retengan los importes de prepago hasta que se registre la factura final. Los prepagos de ventas deben registrarse en una cuenta de pasivos hasta que se envíen los productos. Los prepagos de compras deben registrarse en una cuenta de activos hasta que se reciban los productos. Además, debe configurar distintas cuentas contables generales para cada identificador del IVA.

## <a name="to-add-prepayment-accounts-to-the-general-posting-setup"></a>Para agregar cuentas de prepago a la configuración de grupos contables  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), introduzca **Configuración grupos contables** y, a continuación, elija el vínculo relacionado.
2. En la ventana **Configuración grupos contables**, rellene los campos siguientes:  

    - **Cuenta prepago ventas**  
    - **Cuenta prepagos compras**  

## <a name="to-set-up-number-series-for-prepayment-documents"></a>Configurar números de serie para documentos de prepago  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Conf. ventas y cobros** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Conf. ventas y cobros**, rellene los campos siguientes:  

   - **Nº fact. prepago registrada**
   - **Nº abono prepago registrado**

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Configuración de compras y pagos** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Conf. compras y pagos:**, rellene los campos siguientes:

    - **Nº fact. prepago registrada**
    - **Nº abono prepago registrado**

> [!NOTE]  
>  Puede utilizar la misma numeración de serie para las facturas de prepago y las facturas normales, o bien utilizar numeraciones de serie distintas. Si utiliza series distintas, éstas no deben solaparse, ya que no debe haber ningún número que se repita en ambas series.  

## <a name="to-set-up-prepayment-percentages-for-items-customers-and-vendors"></a>Definir porcentajes de prepago para productos, clientes y vendedores  
Puede definir un porcentaje de prepago predeterminado de un producto para todos los clientes, un cliente determinado o un grupo de precios de cliente.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione un elemento y, a continuación, elija la acción **Conf. ventas y cobros**.  
3. En la ventana **Porcentajes prepago ventas**, rellene los campos como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Puede definir un porcentaje de prepago predeterminado para un cliente o proveedor en relación con todos los productos y todos los tipos de líneas de venta. Especifíquelo en la ficha de cliente o de proveedor.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.
2. Abrir la ficha para un cliente.
3. Rellene el campo **% prepago**.
4. Repita los pasos para otros clientes o proveedores.  

### <a name="to-determine-which-prepayment-percentage-has-first-priority"></a>Para determinar qué porcentaje de prepago tiene prioridad  
Un pedido puede tener un porcentaje de prepago en la cabecera de venta y otro porcentaje distinto para los productos en las líneas. Para determinar qué porcentaje de prepago se aplica a cada línea de venta, el sistema busca el porcentaje de prepago en el siguiente orden y aplicará el primer valor predeterminado que encuentre:  
1. Un porcentaje de prepago para el producto en la línea y el cliente al que se dirige el pedido.  
2. Un porcentaje de prepago para el producto en la línea y el grupo de precios al que pertenece el cliente.  
3. Un porcentaje de prepago para el producto en la línea para todos los clientes.  
4. El porcentaje de prepago en la cabecera de ventas o de compra.  

Dicho de otro modo, el porcentaje de prepago de la ficha del cliente sólo se aplicará si no hay definido un porcentaje de prepago para el producto. Sin embargo, si modifica el contenido del campo **Porcentaje de prepago** en la cabecera de venta o compra después de crear las líneas, se actualizará el porcentaje de prepago en todas las líneas. Esto facilita la creación de un pedido con un porcentaje de prepago fijo, independientemente del porcentaje definido para los productos.

## <a name="see-also"></a>Consulte también  
[Facturación de prepagos](finance-invoice-prepayments.md)  
[Tutorial: Configuración y facturación de prepagos de ventas](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finanzas](finance.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

