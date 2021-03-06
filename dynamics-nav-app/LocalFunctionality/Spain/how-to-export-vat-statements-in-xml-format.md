---
title: Exportar declaraciones de IVA en formato XML
description: "Puede exportar una declaración de IVA en formato XML y después enviarla electrónicamente a las autoridades fiscales."
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
ms.openlocfilehash: 4b9222b6b5fab0d9ef6e8c96ede61b9faf767d7a
ms.contentlocale: es-es
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-export-vat-statements-in-xml-format"></a>Exportar declaraciones de IVA en formato XML
Puede exportar una declaración de IVA en formato XML y después enviarla electrónicamente a las autoridades fiscales.  

Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).  

## <a name="to-export-a-vat-statement-in-xml-format"></a>Para exportar declaraciones de IVA en formato XML  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Declaración del IVA** y, a continuación, seleccione el vínculo apropiado.  
2.  Seleccione la declaración de IVA requerida y después seleccione **Generar archivo XML**.  

    > [!IMPORTANT]  
    >  El nombre de la declaración de IVA debe ser de tipo de plantilla **Informe 1 columna**.  
    >   
    >  En la versión estándar de [!INCLUDE[navnow](../../includes/navnow_md.md)], el nombre de la declaración del IVA para la declaración telemática 392 es del tipo **Informe 1 columna**.  

3.  En la ficha desplegable **Declaración IVA en XML** de la ventana **Modelo 340**, rellene los campos tal y como se describe en la tabla siguiente.  
  
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

