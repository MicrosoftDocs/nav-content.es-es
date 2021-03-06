---
title: "Cambiar el aspecto de un informe seleccionando otro diseño"
description: "Puede utilizar diseños distintos para un informe y cambiar de un diseño a otro para cambiar el aspecto de un informe."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7fc680503a3fb2d685758b69e123dc98b2d98e75
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-change-which-layout-is-currently-used-on-a-report"></a>Cambiar el diseño que se usa actualmente en un informe
Un informe se puede configurar con varios diseños de informe, entre los que puede cambiar según sea necesario.

Según los diseños disponibles para un informe, puede optar por usar un diseño de informe de RDLC integrado, un diseño de informe de Word integrado o un diseño personalizado. Para obtener más información acerca de los diseños de informe de RDLC y de Word, diseños personalizados e integrados y otros temas, consulte [Gestionar diseños de informe](ui-manage-report-layouts.md).

## <a name="to-change-the-layout-that-is-used-on-a-report"></a>Para cambiar el diseño que se usa en un informe
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Selección de diseño de informes** y, a continuación, seleccione el vínculo relacionado.  
   La ventana **Selección de diseño de informes** muestra todos los informes disponibles en la empresa especificada en el campo Empresa en la parte superior de la ventana. El campo Diseño seleccionado especifica el diseño que actualmente se está usando en el informe.
2. Establezca el campo **Empresa** en la parte superior de la ventana en la empresa que incluye el informe.
3. Para cambiar el diseño que se usa en un informe, en la fila del informe en la lista, establezca el campo **Diseño seleccionado** en una de las opciones siguientes:
   * Usa el diseño de informe de RDLC integrado en el informe.
   * Usa el diseño de informe de Word integrado en el informe.
   * Custom, usa un diseño personalizado en el informe.  
     Puede ver qué diseños personalizados estarán disponibles para el informe en el cuadro informativo Parte de diseños de informe. Si no hay diseños personalizados para el informe, deberá crear uno primero. Si elige esta opción, vaya al procedimiento siguiente para especificar el diseño personalizado que desea usar.

    > [!NOTE]  
    >   Si elige **RDLC (integrado)** o **Word (integrado)** y recibe un mensaje de error en el que se indica que el informe no tiene un diseño del tipo especificado, debe elegir otra opción de diseño o crear un diseño de informe personalizado del tipo que desea usar.

Si ha seleccionado un diseño de informe de RDLC o de Word, no se requiere ninguna otra acción y el diseño se utilizará la próxima vez que se ejecute el informe.

## <a name="to-specify-a-custom-layout-on-a-report"></a>Para especificar un diseño personalizado en un informe
1. El diseño personalizado que se usará en el informe se especifica en la ventana **Diseños de informe personalizados**. Si la ventana **Diseños de informes personalizados** no está abierta, seleccione el botón de búsqueda en el campo **Descripción de diseño de informe**.
2. En la ventana **Diseños de informe personalizados**, seleccione la fila del diseño personalizado que desee usar y, a continuación, cierre la ventana.

Puede volver a la ventana **Selección de diseño de informes**. El nombre del diseño personalizado seleccionado se muestra en el campo **Descripción de diseño personalizado**. El diseño personalizado se utilizará la siguiente vez que se ejecute el informe.

## <a name="see-also"></a>Consulte también
[Gestión de diseños de informe](ui-manage-report-layouts.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

