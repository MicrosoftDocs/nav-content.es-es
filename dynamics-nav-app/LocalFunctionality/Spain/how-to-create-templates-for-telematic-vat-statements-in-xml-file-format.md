---
title: "Crear plantillas para las declaraciones telemáticas de IVA en formato XML"
description: "Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios. Puede enviar los archivos en formato de texto y en formato XML. Este procedimiento describe cómo crear plantillas para los archivos XML."
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
ms.openlocfilehash: 30f5798425cf082b6361441e98feede6af58a68d
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-templates-for-telematic-vat-statements-in-xml-file-format"></a>Crear plantillas para las declaraciones telemáticas de IVA en formato XML
Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios. Puede enviar los archivos en formato de texto y en formato XML. Este procedimiento describe cómo crear plantillas para los archivos XML.  
  
 Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  
  
### <a name="to-create-a-template-for-vat-statements-in-xml-file-format"></a>Para crear una plantilla para las declaraciones telemáticas de IVA en formato de archivo XML  
  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Declaración del IVA** y, a continuación, seleccione el vínculo apropiado.  
  
2.  Seleccione la declaración de IVA requerida y luego, en la pestaña **Acciones**, elija **IVA telemático**, y **Diseñar archivo XML**.  
  
3.  En la ventana **Formato transferencia XML**, rellene los campos tal como se describe en la tabla siguiente.  
  
    > [!IMPORTANT]  
    >  Los valores de los campos están determinados por las autoridades fiscales.  
    >   
    >  Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  
  
    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nombre decl. IVA**|Especifique el nombre de la declaración del IVA para el que está diseñada esta plantilla.|  
    |**Nº**|Especifique el número de campo en el archivo de texto.|  
    |**Tipo de línea**|Especifique si el tipo de línea de la declaración del IVA es un elemento XML o un atributo XML.|  
    |**Nivel sangría**|Especifique el nivel de sangría de la etiqueta. Este nivel se utiliza para formatear el archivo XML.|  
    |**Nº línea maestro**|Especifique el número de línea de la línea principal con la que se sangra la línea actual.|  
    |**Tipo de valor**|Especifique el subtipo del campo.<br /><br /> El subtipo especifica si la línea debe mostrar solo la parte entera de un importe, la parte decimal, o el importe total.|  
    |**Descripción**|Especifique el texto que desea que aparezca en la etiqueta.|  
    |**Valor**|Especifique el valor de la etiqueta.|  
    |**Caja**|Especifique el número de casilla desde donde recuperar los datos.|  
    |**Preguntar**|Especifica si el campo **Valor** se puede modificar antes de crear el archivo XML.|  
    |**Existe importe**|Seleccione esta opción para incluir el importe existente.|  
  
4.  Repita el paso anterior para las líneas adicionales en la declaración de IVA.  
  
5.  Elija el botón **Aceptar**.  
  
 Esta acción crea la plantilla. Ahora puede crear un archivo que luego puede enviar a las autoridades fiscales.  
  
## <a name="see-also"></a>Consulte también  
 [Exportar declaraciones de IVA en formato XML](how-to-export-vat-statements-in-xml-format.md)   
 [Crear plantillas para las declaraciones telemáticas de IVA en formato de archivo de texto](how-to-create-templates-for-telematic-vat-statements-in-text-file-format.md)   
 Formato XML de transferencia AEAT
