---
title: "Recibir y convertir documentos electrónicos"
description: "Puede recibir documentos electrónicos directamente desde sus socios colaboradores o desde un servicio de OCR."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 889fe150eb96a02569e057d5830164630dc20812
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-receive-and-convert-electronic-documents"></a>Procedimiento: recibir y convertir documentos electrónicos
La versión genérica de [!INCLUDE[d365fin](includes/d365fin_md.md)] admite la recepción de facturas electrónicas y abonos en formato PEPPOL, admitido por los proveedores de servicios de intercambio de documentos más importantes. Para recibir una factura de un proveedor como un documento electrónico PEPPOL, debe procesarse el documento en la ventana Documentos entrantes para luego convertirlo en una factura de compra o en una línea de diario general en [!INCLUDE[d365fin](includes/d365fin_md.md)].

 Además de recibir documentos electrónicos directamente de los socios comerciales, puede recibir documentos electrónicos de un servicio OCR que haya convertido sus archivos PDF o de imagen en documentos electrónicos.  

 Antes de que pueda recibir documentos electrónicos a través del servicio de intercambio de documentos, debe configurar los distintos datos maestros, como la información de empresa, proveedores, artículos y unidades de medida. Se utilizan para identificar a los socios comerciales y los productos al convertir los datos de elementos del archivo de documento entrante en campos de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Para obtener más información, vea [Procedimiento: Configurar un servicio de intercambio de documentos](across-how-to-set-up-a-document-exchange-service.md).  

 Antes de que pueda recibir documentos electrónicos a través del servicio OCR, debe configurar y habilitar la conexión de servicio preconfigurada. Para obtener más información, vea [Procedimiento: Configurar documentos entrantes](across-how-setup-income-documents.md).  

 El tráfico de documentos electrónicos hacia y desde [!INCLUDE[d365fin](includes/d365fin_md.md)] lo administra la característica Cola proyecto. Antes de que pueda recibir documentos electrónicos, debe iniciarse la cola de proyectos correspondiente.  

 Puede iniciar la conversión de documentos electrónicos manualmente, tal como se describe en este procedimiento, o puede activar un flujo de trabajo para convertir los documentos electrónicos automáticamente cuando se reciban. La versión genérica de [!INCLUDE[d365fin](includes/d365fin_md.md)] incluye una plantilla de flujo de trabajo, *Flujo de trabajo desde Documento electrónico entrante hasta Abrir factura de compra*, que está listo para copiarse en un flujo de trabajo y activarse. Para obtener más información, consulte [Flujo de trabajo](across-workflow.md).  

> [!NOTE]  
>  Cuando conviertes documentos electrónicos recibidos del servicio de OCR o de líneas del diario de [!INCLUDE[d365fin](includes/d365fin_md.md)], se suman varias líneas en el documento de origen en una línea. La línea única será del tipo Cuenta del libro mayor y los campos de **Descripción** y **Número** (de cuenta del libro mayor) estarán vacíos. El valor del campo **Importe** se igualará al importe total (IVA excluido) de todas las líneas del documento de origen.  
>   
>  Para asegurarse de que los campos **Descripción** y **N.º** se rellenan, puede elegir el botón **Asignar texto a cuenta** en la ventana **Documentos entrantes** para definir que un determinado texto de factura se asigne siempre a una cuenta Debe o Haber determinada en la contabilidad. En adelante, el campo **Descripción** del documento o de las líneas de diario creados a partir de un documento electrónico para el proveedor o cliente en concreto se rellenarán con el texto en cuestión y el campo **N.º** (cuenta libro mayor) con la cuenta en cuestión.  
>   
>  En lugar de asignar a una cuenta, también se puede asignar a una cuenta bancaria. Esto resulta práctico, por ejemplo, en los documentos electrónicos para los gastos que ya se han pagado, donde desea crear una línea de diario general que esté lista para registrarse en una cuenta bancaria.  

 El procedimiento siguiente describe cómo recibir una factura de proveedor y convertirla en una factura de compra en [!INCLUDE[d365fin](includes/d365fin_md.md)]. El procedimiento es el mismo cuando se convierte una factura de proveedor en una línea de diario general.  

### <a name="to-receive-and-convert-an-electronic-invoice-to-a-purchase-invoice"></a>Para recibir y convertir una factura electrónica en una factura de compra  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Documentos entrantes** y, a continuación, seleccione el vínculo relacionado.  

2.  Seleccione la línea del registro del documento entrante que representa una factura electrónica entrante nueva y, en la pestaña **Inicio**, en el grupo **Administrar**, elija **Editar**.  

     En la ventana **Ficha de documento entrante**, está adjunto el archivo XML relacionado, y la mayor parte de los campos se prellenan con la información de la factura electrónica. Para obtener más información, vea [Procedimiento: Crear registros de documentos entrantes](across-how-create-income-document-records.md).  

3.  En el campo **Tipo de intercambio de datos**, seleccione **PEPPOL - Factura** o **OCR - Factura** según el origen del documento electrónico.  

4.  Para asignar el texto de la factura de proveedor a una cuenta Debe específica, en la pestaña **Acciones**, en el grupo **General**, seleccione **Asignar texto a cuenta** y, a continuación rellene la ventana **Hoja asignación de texto a cuenta**.  

5.  En la ventana **Acciones**, en el grupo **General**, elija **Crear documento**.  

     Se creará una factura de compra en [!INCLUDE[d365fin](includes/d365fin_md.md)] basándose en la información del documento electrónico.  

     Los errores de validación, normalmente relacionados con datos maestros incorrectos o no presentes en [!INCLUDE[d365fin](includes/d365fin_md.md)], se mostrarán en la ficha desplegable **Mensajes de error**.  

## <a name="see-also"></a>Consulte también  
[Gestionar pagos](payables-manage-payables.md)  
[Documentos entrantes](across-income-documents.md)  
[Procedimiento: Configurar el envío y la recepción de documentos electrónicos](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[Intercambio de datos electrónicamente](across-data-exchange.md)   
[Funciones empresariales generales](ui-across-business-areas.md)  

