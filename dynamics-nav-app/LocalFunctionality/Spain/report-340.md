---
title: Informe 340
description: "El Informe 340 contiene información sobre facturas e impuestos emitidos o recibidos por su empresa en un período determinado. El informe se genera en un formato que ha aprobado la administración fiscal."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 977d43693a90554c0a344ddb3b0f320aaabd0dca
ms.contentlocale: es-es
ms.lasthandoff: 10/26/2017

---
# <a name="report-340"></a>Informe 340
El **Informe 340** contiene información sobre facturas e impuestos emitidos o recibidos por su empresa en un período determinado. El informe se genera en un formato que ha aprobado la administración fiscal. Este informe debe enviarse en el período de liquidación mensual o trimestral de la empresa, según el tamaño de la empresa. Este archivo puede cargarse en el sitio web de la Agencia Tributaria o enviarse en CD-ROM. Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://www.aeat.es/wps/portal/Home?channel=1af861cd949a1010VgnVCM100000d7005a80____&ver=L&site=56d8237c0bc1ff00VgnVCM100000d7005a80____&idioma=es_ES&menu=0&img=0). Si el número de operaciones es mayor a 1 000 000 el informe se puede enviar electrónicamente.  

## <a name="reporting-requirements-for-entrepreneurs-and-small-companies"></a>Requisitos de informes para emprendedores y pequeñas empresas  
Los requisitos de presentación de informes para empresarios y pequeñas empresas se modifican para apoyar a las empresas que utilizan los criterios de contabilidad de efectivo (CAC).  

Una empresa puede utilizar el método de contabilidad de efectivo si las ventas del negocio no exceden los 2 millones de euros al año. Hay una excepción a esta regla para una empresa cuyos recibos en efectivo de un único cliente exceden la suma de 100 000 euros.  

En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede configurar grupos de contabilización para la contabilización del IVA en efectivo para compras y ventas.  

 Si se archiva un informe de este régimen, se aplica la etiqueta siguiente a algunos informes de [!INCLUDE[navnow](../../includes/navnow_md.md)]: **Régimen especial del criterio de caja**. Los informes modificados son:  

|Informe|Description|  
|------------|---------------------------------------|  
|Informe 117|Recordatorio|  
|Informe 118|Documento de interés|  
|Informe 205|Confirmación pedido|  
|Informe 206|Ventas - Factura|  
|Informe 207|Ventas - Abono|  
|Informe 405|Pedido compra|  
|Informe 406|Compra – Factura|  
|Informe 407|Compras - Abono|  
|Informe 5900|Pedido servicio|  
|Informe 5911|Servicio - Factura|  
|Informe 5912|Servicio - Abono|  

## <a name="file-format"></a>Formato de archivo  
El formato de archivo del **informe 340** incluye un registro de deponente y al menos una de las facturas emitidas y facturas recibidas. La información de deponente se obtiene de la tabla **Información empresa** y del formulario de solicitud. Las facturas emitidas se obtienen de las empresas a las que se han vendido mercancías o servicios. La información de cliente se obtiene de la tabla **Cliente**. Las facturas recibidas se obtienen de las empresas a las que se han comprado mercancías o servicios. La información de proveedor se obtiene de la tabla **Proveedor**.  

> [!NOTE]  
>  Si no hay ningún registro de formato, el archivo no se crea y se muestra un mensaje de error.  

## <a name="entries-included-in-report-340"></a>Movimientos incluidos en el informe 340  
Los movimientos incluidos en el **informe 340** deben haberse registrado durante el ejercicio y el periodo que se ha indicado en el formulario de solicitud. Los movimientos que se incluyen en el informe de pagos en efectivo se pueden registrar del año anterior.  

### <a name="businesses"></a>Negocios  
El **Informe 340** debe incluir los siguientes movimientos:  

- Facturas de ventas y abonos registrados.  
- Facturas de compras y abonos registrados.  
- Facturas de servicios y abonos registrados.  
- Autofacturas y autoabonos.  
- Pagos en efectivo.  

Los movimientos del informe **Libro facturas emitidas** se deben incluir en el informe como facturas emitidas.  

Los movimientos del informe **Libro facturas recibidas** se deben incluir en el informe como facturas recibidas.  

### <a name="small-businesses"></a>Empresas pequeñas  
Para las pequeñas empresas y los empresarios que operan bajo los Criterios de contabilidad de efectivo (CAC), el Informe 340 informa de las facturas en virtud del CAC. La factura está marcada con una “Z” para el tipo de la operación. Si la factura está bajo el CAC, se informa de lo siguiente:  

- Método de pago/recibo, es decir, efectivo, cheque, transferencia, etc. Si no se ha producido ningún cobro, este campo estará en blanco en el informe.  
- Importe pago/albarán (completo, parcial)  
- Fechas pagos/albarán  

### <a name="invoices-including-different-vat-percentages-or-ec-percentages"></a>Facturas con diferentes porcentajes de IVA o de RE  
Si la factura tiene más de un porcentaje de IVA o de recargo de equivalencia (RE), el informe debe incluir todos los registros con diferentes porcentajes de IVA y RE. Si la factura incluye recargos de equivalencia (RE), se mostrará el porcentaje de RE y el importe de RE sin IVA.  

En todos los registros se mostrará el mismo Id. de factura y número de IVA del cliente.  

## <a name="file-format-restrictions"></a>Restricciones del formato de archivo  
Antes de crear el informe **Informe 340**, debe tener en cuenta las siguientes restricciones de formato de archivo:  

- Todos los importes se deben expresar en euros.  
- Todos los importes deben ser positivos. En los campos donde son posibles importes negativos, se indica **N**.  
- Todo el texto deber estar en mayúsculas.  
- Todos los campos alfanuméricos se deben alinear a la izquierda.  
- Todos los campos numéricos deben ir alineados a la derecha.  
- Los caracteres especiales se convierten a caracteres estándar.  
- Si no contienen ningún valor, los campos alfanuméricos se dejarán en blanco y los campos numéricos se rellenarán con ceros.  

## <a name="see-also"></a>Consulte también  
 [Creación del informe 340](how-to-create-report-340.md)   
 [Pagos en efectivo](payments-in-cash.md)   
 [Funcionalidad local para España](spain-local-functionality.md)

