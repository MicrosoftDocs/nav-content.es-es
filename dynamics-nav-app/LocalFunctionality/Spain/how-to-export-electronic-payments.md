---
title: "Exportar pagos electrónicos"
description: "En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede exportar movimientos del diario de pagos a un formato de archivo de acuerdo con cuatro estándares de pago diferentes. Utilice las siguientes ventanas para exportar según los distintos estándares de pago."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: d0b9763052820326aa7b294b0bd6f67771937525
ms.contentlocale: es-es
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-export-electronic-payments"></a>Exportar pagos electrónicos
En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede exportar movimientos del diario de pagos a un formato de archivo de acuerdo con cuatro estándares de pago diferentes. Utilice las siguientes ventanas para exportar según los distintos estándares de pago.  

|Estándar de pago|Ventana desde la que exportar|  
|----------------------|---------------------------|  
|AEB N34|**Ordenes pago**|  
|AEB N34.1|**Ordenes pago**|  
|PAGO ELECTRÓNICO|**Diario de pagos**|  
|SEPA|**Diario de pagos** u **Órdenes pago**|  

> [!IMPORTANT]  
>  Antes de exportar un pago, debe seleccionar un formato de pago en el campo **Formato de exportación de pagos** en la ventana **Ficha banco**.  

## <a name="to-export-electronic-payments-using-the-payment-orders-window"></a>Para exportar pagos electrónicos mediante la ventana Órdenes de pago  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Órdenes pago** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione los documentos que desea pagar.  
3.  Seleccione la acción **Exportar a archivo**.  

    Los pagos de tipo SEPA se exportarán a un archivo inmediatamente.  

    Los pagos de tipo N34 o N34.1 se exportarán cuando ejecute el informe **Orden pago - Exportar N34** u **Orden pago - Exportar N34.1**, que se muestran automáticamente cuando selecciona **Exportar** en el paso 3.  

4.  En la ventana **Orden pago - Exportar N34.1**, rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**N.º cuenta bancaria**|Seleccione el código de cuenta desde la que se van a exportar los pagos.|  
    |**Fecha liquidación**|Especifique la fecha en la que la exportación se transmitirá al banco. Esta fecha será la fecha de registro de los movimientos exportados del diario de pagos.|  
    |**Si Fecha registro no coincide con Fecha de emisión**|Especifique si desea que la fecha de liquidación coincida o si desea omitir las líneas de diario de pagos cuya fecha de registro no coincida con la fecha de liquidación.|  
    |**Código gastos**|Especifique el responsable de los gastos de pago.|  
    |**Compartido (sólo transf. internacionales).**|Especifique si desea que el pagador y el beneficiario compartan los gastos. Solo se puede usar en transferencias internacionales.|  
    |**Concepto orden pago.**|Especifique el concepto de orden de pago, **Nómina**, **Nómina pensión** u **Otros**.|  
    |**Relación**|Especifique si desea que el banco le envíe una lista detallada de los cargos por transferencias. Si no selecciona este campo, el banco le enviará el total de todos los cargos de todas las transferencias realizadas.|  
    |**Número copias**|Especifique el número de copias adicionales del aviso de pago que se imprimirán mediante este proceso. Siempre se imprime un documento para que se pueda enviar al beneficiario.|  

5.  Seleccione la acción **Imprimir** o **Vista previa** para ver el archivo de pagos creado.  

    Se exportarán los movimientos del diario de pagos cuyo campo **Tipo pago por banco** esté establecido en **Pago electrónico**. Los datos se exportarán a un archivo con el formato estándar N34 o N34.1. Además, se imprimirá un aviso de pago adecuado para su envío a cada beneficiario.  

    > [!NOTE]  
    >  Solo puede registrar la orden de pago una vez que haya exportado correctamente los pagos electrónicos.  

## <a name="to-export-electronic-payments-using-the-payment-journal-window"></a>Para exportar pagos electrónicos mediante la ventana Diario de pagos  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios de pagos** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione los documentos que desea pagar.  
3.  En la pestaña **Navegar**, elija **Pagos electrónicos** y después seleccione **Exportar**.  

    Los pagos de tipo SEPA se exportarán a un archivo inmediatamente.  

    Los pagos de tipo E-PAY se exportarán cuando ejecute el informe **Exportar pagos electrónicos**, que se muestran automáticamente cuando selecciona **Exportar** en el paso 3.  

4.  En la ventana **Exportar pagos electrónicos**, rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**N.º cuenta bancaria**|Seleccione el código de cuenta desde la que se van a exportar los pagos.|  
    |**Fecha liquidación**|Especifique la fecha en la que la exportación se transmitirá al banco. Esta fecha será la fecha de registro de los movimientos exportados del diario de pagos.|  
    |**Si Fecha registro no coincide con Fecha de emisión**|Especifique si desea que la fecha de liquidación coincida o si desea omitir las líneas de diario de pagos cuya fecha de registro no coincida con la fecha de liquidación.|  
    |**Código gastos**|Especifique el responsable de los gastos de pago.|  
    |**Compartido (sólo transf. internacionales).**|Especifique si desea que el pagador y el beneficiario compartan los gastos. Solo se puede usar en transferencias internacionales.|  
    |**Concepto orden pago.**|Especifique el concepto de orden de pago, **Nómina**, **Nómina pensión** u **Otros**.|  
    |**Relación**|Especifique si desea que el banco le envíe una lista detallada de los cargos por transferencias. Si no selecciona este campo, el banco le enviará el total de todos los cargos de todas las transferencias realizadas.|  
    |**Número copias**|Especifique el número de copias adicionales del aviso de pago que se imprimirán mediante este proceso. Siempre se imprime un documento para que se pueda enviar al beneficiario.|  

5.  Seleccione la acción **Imprimir** o **Vista previa** para ver el archivo de pagos creado.  

    Se exportarán los movimientos del diario de pagos cuyo campo **Tipo pago por banco** esté establecido en **Pago electrónico**. Los datos se exportarán a un archivo con el formato estándar del pago seleccionado. Además, se imprimirá un aviso de pago adecuado para su envío a cada beneficiario.  

    > [!NOTE]  
    >  Solo puede registrar la orden de pago una vez que haya exportado correctamente los pagos electrónicos.  

    > [!NOTE]  
    >  En la versión genérica de [!INCLUDE[navnow](../../includes/navnow_md.md)], la ventana **Diario de pagos** se utiliza de forma similar para exportar pagos electrónicos en el formato de transferencia de crédito SEPA. Para obtener más información, consulte [Realizar pagos con Servicio de conversión de datos del banco o Transferencia de crédito SEPA](../../finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md).  

## <a name="to-export-electronic-payments-from-the-cartera-module"></a>Para exportar los pagos electrónicos del módulo Cartera  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Orden pago - Exportar N34.1** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Fecha de emisión**|Especifique la fecha de entrega de pago electrónico.|  
    |**Código gastos**|Especifique el responsable de los gastos de pago.|  
    |**Concepto orden pago**|Especifique el concepto de orden de pago, **Nómina**, **Nómina pensión** u **Otros**.|  
    |**Relación**|Especifique si desea que el banco le envíe una lista detallada de los cargos por transferencias. Si no selecciona este campo, el banco le enviará el total de todos los cargos de todas las transferencias realizadas.|  
    |**Número copias**|Especifique el número de copias adicionales del aviso de pago que se imprimirán mediante este proceso. Siempre se imprime un documento para que se pueda enviar al beneficiario.|  
    |**Compartido (solo transf. internacionales)**|Especifique si desea que el pagador y el beneficiario compartan los gastos. Solo se puede usar en transferencias internacionales.|  

> [!NOTE]  
>  Solo puede registrar la orden de pago una vez que haya exportado correctamente los pagos electrónicos.  

## <a name="see-also"></a>Consulte también  
 [Pagos electrónicos – AEB N34.1](electronic-payments-aeb-n34.1.md)   
 Exportar pagos electrónicos   
 [Configurar cuentas bancarias para realizar pagos electrónicos](how-to-set-up-bank-accounts-for-electronic-payments.md)   
 [Realizar pagos con Servicio de conversión de datos del banco o Transferencia de crédito SEPA](../../finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)

