---
title: "Crear plantillas para las declaraciones telemáticas de IVA en formato de archivo de texto"
description: "Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios. Puede enviar los archivos en formato de texto y en formato XML. Este procedimiento describe cómo crear plantillas para los archivos de texto."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3dd1e8ac5db93ca738a1c3ad76131038cd8abef7
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-templates-for-telematic-vat-statements-in-text-file-format"></a>Crear plantillas para las declaraciones telemáticas de IVA en formato de archivo de texto
Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios. Puede enviar los archivos en formato de texto y en formato XML. Este procedimiento describe cómo crear plantillas para los archivos de texto.  
  
 Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  
  
### <a name="to-create-a-template-for-vat-statements-in-text-file-format"></a>Para crear una plantilla para las declaraciones telemáticas de IVA en formato de archivo de texto  
  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Declaración del IVA** y, a continuación, seleccione el vínculo apropiado.  
  
2.  Seleccione la declaración de IVA requerida y luego, en la pestaña **Acciones**, elija **IVA telemático**, y **Diseñar archivo txt**.  
  
3.  En la ventana **Formato transferencia**, rellene los campos tal como se describe en la tabla siguiente.  
  
    > [!IMPORTANT]  
    >  Los valores de los campos están determinados por las autoridades fiscales.  
    >   
    >  Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  
  
    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nombre decl. IVA**|Especifique el nombre de la declaración del IVA para el que está diseñada esta plantilla.|  
    |**Nº**|Especifique el número de campo en el archivo de texto.|  
    |**Posición**|Especifique la posición de este campo en el archivo de texto.|  
    |**Longitud**|Especifique la longitud del campo.|  
    |**Escriba**|Especifique el tipo del campo. Las opciones disponibles son **Alfanumérico**, **Numérico**, **Fijo**, **Preguntar** y **Divisa**.|  
    |**Subtipo**|Especifique el subtipo del campo.<br /><br /> El subtipo especifica si la línea debe mostrar solo la parte entera de un importe, la parte decimal, o el importe total.|  
    |**Descripción**|Especifique el texto que desea que aparezca en la etiqueta.|  
    |**Valor**|Especifique el valor de la etiqueta.|  
    |**Caja**|Especifique el número de casilla desde donde recuperar los datos.|  
  
4.  Repita el paso anterior para las líneas adicionales en la declaración de IVA.  
  
5.  Elija el botón **Aceptar**.  
  
 Esta acción crea la plantilla. Ahora puede crear un archivo que luego puede enviar a las autoridades fiscales.  
  
## <a name="see-also"></a>Consulte también  
 [Exportar declaraciones de IVA en formato de texto](how-to-export-vat-statements-in-text-format.md)   
 [Crear plantillas para las declaraciones telemáticas de IVA en formato XML](how-to-create-templates-for-telematic-vat-statements-in-xml-file-format.md)   
 Formato transfer. AEAT
