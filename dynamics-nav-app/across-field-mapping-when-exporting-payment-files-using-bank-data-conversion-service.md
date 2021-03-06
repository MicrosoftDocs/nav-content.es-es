---
title: "Asignación de campos para exportar los archivos de pago de banco"
description: "Cuando se exportan archivos de pago con la función de servicio de conversión de datos bancarios, los datos exportados serán visibles para el proveedor del servicio de conversión de datos bancarios."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 7eebca3303e9844e4ec8be2940104f9cb7216f6a
ms.contentlocale: es-es
ms.lasthandoff: 10/23/2017

---
# <a name="field-mapping-when-exporting-payment-files-using-bank-data-conversion-service"></a>Asignación de campos al exportar archivos de pago con el servicio de conversión de datos bancarios
Cuando se exportan archivos de pago con la función de servicio de conversión de datos bancarios, los datos exportados serán visibles para el proveedor del servicio de conversión de datos bancarios. El proveedor del servicio es responsable de la privacidad de estos datos. Para obtener más información sobre la función de servicio de conversión de datos bancarios, consulte [Acerca del marco de intercambio de datos](across-about-the-data-exchange-framework.md).  

> [!CAUTION]  
>  Cuando se exportan archivos de pago con la función de servicio de conversión de datos bancarios, algunos de los datos empresariales serán visibles para el proveedor del servicio. El proveedor de servicios, AMC Consult A/S, es responsable de la privacidad de estos datos. Para obtener más información, consulte [Directiva de función de AMC](http://go.microsoft.com/fwlink/?LinkId=510158).  

La tabla siguiente indica los campos de [!INCLUDE[d365fin](includes/d365fin_md.md)] desde los que se pueden exportar datos al proveedor de servicios.  

|Campo asignado|Campo en tabla|Escritorio|Description|  
|------------------|--------------------|-----------|---------------------------------------|  
|N.º acreedor|N.º acreedor|Cuenta bancaria|El identificador asignado a su empresa por el banco para cobrar a los pagos|  
|N.º de cuenta bancaria del remitente|N.º cuenta bancaria/IBAN|Cuenta bancaria|El número de la cuenta bancaria de su empresa (IBAN u otro) que se especifica en la ficha de la cuenta bancaria|  
|Estándar de compensación bancaria del remitente|Estándar de compensación bancaria|Cuenta bancaria|El registro de nombres de bancos nacionales utilizado para la cuenta bancaria del emisor|  
|Código de compensación del banco del remitente|Código de compensación bancaria|Cuenta bancaria|El identificador del banco del remitente en relación con el registro de nombres de bancos utilizado|  
|BIC del banco del remitente|Código SWIFT|Cuenta bancaria|El identificador SWIFT de la cuenta bancaria del emisor.|  
|Divisa de cuenta bancaria del remitente|Cód. divisa|Cuenta bancaria|El código de divisa de la cuenta bancaria del remitente|  
|Nº documento|Nº documento|Línea diario general|El número de documento de la línea de pago|  
|Liq. por nº doc. externo|Liq. por nº doc. externo|Línea diario general|El número de documento externo de la factura o del abono al que se aplica la línea de pago.|  
|Id. del destinatario|Nº cuenta|Línea diario general|El número de cliente o proveedor especificado en la línea de pago|  
|Tipo pago|Conversión de datos del banco - Tipo de pagos|Forma pago|El tipo de transferencia bancaria, como nacional o internacional|  
|Referencia pago|Referencia pago|Línea diario general|La referencia de pago de la línea de pago|  
|Dirección del destinatario|Dirección|Cliente/Proveedor|La dirección del receptor especificada en la ficha de cliente o de proveedor|  
|Ciudad del destinatario|Población|Cliente/Proveedor|La población del receptor especificada en la ficha de cliente o de proveedor|  
|Nombre del destinatario|Nombre|Cliente/Proveedor|El nombre del receptor especificado en la ficha de cliente o de proveedor|  
|Código de país/región del destinatario|Cód. país/región|Cliente/Proveedor|El código de país o región del receptor especificado en la ficha de cliente o de proveedor|  
|Código postal del destinatario|C.P.|Cliente/Proveedor|El código postal del receptor especificado en la ficha de cliente o de proveedor|  
|N.º cta. bancaria destinatario|N.º cuenta bancaria/IBAN|Banco cliente/Banco proveedor|El número de la cuenta bancaria del receptor (IBAN u otro) que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|Código de compensación del banco del destinatario|Estándar de compensación bancaria|Banco cliente/Banco proveedor|El registro de nombres de bancos nacionales utilizado para la cuenta bancaria del receptor|  
|Est. de compensación del banco del destinatario|Código de compensación bancaria|Banco cliente/Banco proveedor|El identificador de la cuenta bancaria del receptor en relación con el registro de nombres de bancos utilizado|  
|Dirección correo elect. del destinatario|E-Mail|Cliente/Proveedor|La dirección de correo electrónico del destinatario|  
|Mensaje al destinatario 1|Mensaje al destinatario|Línea diario general|El mensaje al receptor especificado en la línea de pago|  
|Importe|Importe|Línea diario general|El importe en la línea de pago|  
|Cód. divisa|Cód. divisa|Línea diario general|El código de divisa en la línea de pago.|  
|Fecha de transferencia|Fecha registro|Línea diario general|La fecha de registro de la línea de pago|  
|Importe factura|Importe inicial|Mov. proveedor/cliente|El importe en el movimiento para el que se liquida el pago.|  
|Fecha factura|Fecha emisión documento|Mov. proveedor/cliente|La fecha de factura en el movimiento para el que se liquida el pago|  
|Dirección del banco del destinatario|Dirección|Banco cliente/Banco proveedor|La dirección de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|La dirección de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|Población|Banco cliente/Banco proveedor|La población de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|Nombre del banco del destinatario|Nombre|Banco cliente/Banco proveedor|El nombre de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|País/región del banco del destinatario|Cód. país/región|Banco cliente/Banco proveedor|El país o la región de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|Código postal del banco destinatario|C.P.|Banco cliente/Banco proveedor|El código postal de la cuenta bancaria del receptor que se especifica en la ficha de la cuenta bancaria del cliente o del proveedor|  
|Dirección del banco del remitente|Dirección|Cuenta bancaria|La dirección de la cuenta bancaria del emisor especificada en la ficha de la cuenta bancaria|  
|Ciudad del banco del remitente|Población|Cuenta bancaria|La población de la cuenta bancaria del emisor especificada en la ficha de la cuenta bancaria|  
|Nombre del banco del remitente|Nombre|Cuenta bancaria|El nombre de la cuenta bancaria del emisor especificada en la ficha de la cuenta bancaria|  
|País/región del banco del remitente|Cód. país/región|Cuenta bancaria|El país o región de la cuenta bancaria del emisor especificada en la ficha de la cuenta bancaria|  
|Código postal del banco del remitente|C.P.|Cuenta bancaria|El código postal de la cuenta bancaria del emisor especificada en la ficha de la cuenta bancaria|  
|Plantilla de libros diario general|Nombre libro diario|Línea diario general|La plantilla de la sección de diario general que se usa para la línea de pago|  
|Nombre sección diario general|Nombre sección diario|Línea diario general|El nombre de la sección de diario general que se usa para la línea de pago|  
|Nombre del banco del remitente - Conv. de datos|Nombre del banco - Conv. de datos|Cuenta bancaria|El nombre de la cuenta bancaria del emisor solicitado por el servicio de conversión de datos bancarios y especificado en la ficha de la cuenta bancaria|  

## <a name="see-also"></a>Consulte también  
[Configuración del intercambio de datos](across-set-up-data-exchange.md)  
[Intercambio de datos electrónicamente](across-data-exchange.md)
[Procedimiento: Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md)   
[Realizar pagos con Servicio de conversión de datos del banco o Transferencia de crédito SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)   

