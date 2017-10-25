---
title: Exportar declaraciones de IVA en formato XML
description: "Puede exportar una declaración de IVA en formato XML y después enviarla electrónicamente a las autoridades fiscales."
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
ms.openlocfilehash: 1438b9d7cb327fccf03012132c52e96459df46a7
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-vat-statements-in-xml-format"></a>Exportar declaraciones de IVA en formato XML
Puede exportar una declaración de IVA en formato XML y después enviarla electrónicamente a las autoridades fiscales.  
  
 Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  
  
### <a name="to-export-a-vat-statement-in-xml-format"></a>Para exportar declaraciones de IVA en formato XML  
  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Declaración del IVA** y, a continuación, seleccione el vínculo apropiado.  
  
2.  Seleccione la declaración de IVA requerida y luego, en la pestaña **Acciones**, elija **IVA telemático**, y **Generar archivo XML**.  
  
    > [!IMPORTANT]  
    >  El nombre de la declaración de IVA debe ser de tipo de plantilla **Informe 1 columna**.  
    >   
    >  En la versión estándar de [!INCLUDE[navnow](../../includes/navnow_md.md)], el nombre de la declaración del IVA para la declaración telemática 392 es del tipo **Informe 1 columna**.  
  
3.  En la ventana **Declaración IVA en XML**, en la ficha desplegable **ADD INCLUDE<!--[!INCLUDE[bp_optionsheading](../../includes/bp_optionsheading_md.md)]-->**, rellene los campos tal y como se describe en la tabla siguiente.  
  
    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Movs. IVA incluidos**|Especifique si la declaración de IVA debe incluir los movimientos pendientes, los cerrados, o ambos.|  
    |**Movs. IVA incluidos**|Especifique si la declaración de IVA debe incluir únicamente los movimientos del periodo que se especifica en el campo **Filtro fecha** o también movimientos de periodos anteriores.|  
    |**Divisa adicional**|Seleccione que se muestren los importes del informe en una divisa adicional de informe.|  
  
4.  En la ficha desplegable **Lín. declaración IVA**, especifique un valor del campo **Filtro fecha**.  
  
     Opcionalmente, seleccione los filtros adicionales.  
  
5.  Elija el botón **Aceptar**.  
  
6.  En la ventana **Formato de transferencia XML**, verifique que la declaración de IVA se configura correctamente y después seleccione el botón **Aceptar**  
  
 Puede abrir o guardar el archivo XML generado. Ahora puede enviar la declaración del IVA a las autoridades fiscales.  
  
## <a name="see-also"></a>Consulte también  
 [Crear plantillas para las declaraciones telemáticas de IVA en formato XML](how-to-create-templates-for-telematic-vat-statements-in-xml-file-format.md)   
 [Exportar declaraciones de IVA en formato de texto](how-to-export-vat-statements-in-text-format.md)   
 Declaración IVA en XML
