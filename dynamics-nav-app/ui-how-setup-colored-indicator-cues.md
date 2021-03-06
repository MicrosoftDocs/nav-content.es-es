---
title: "Especificar los indicadores de color para personalizar las señales visuales acerca de la actividad de una pila"
description: "Configure un indicador de color en un mosaico Pila para proporcionar una señal visual personalizada de la actividad de la pila."
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6a2b7deb2f256e3b6bf52f1b0a66fe47d049c452
ms.contentlocale: es-es
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>Procedimiento: Configurar un indicador de color en pilas
Puede configurar pilas para que aparezcan en la página **Inicio** a fin de que incluyan un indicador que cambia de color según los valores de datos de las pilas.

El indicador se muestra como una barra de color a lo largo del borde superior del mosaico de la pila. Proporciona una guía visual del estado de la actividad de la pila, que puede indicar condiciones favorables o desfavorables para que el usuario actúe en consecuencia. Por ejemplo, si una pila muestra las facturas de venta en curso, puede configurar que el indicador aparezca de color verde (favorable) si el número total de facturas de venta en curso es inferior a 10 y que aparezca de color rojo (desfavorable) si el total es mayor que 20.

En la ventana **Configuración de pila** se configuran indicadores para todas las pilas que están disponibles en la base de datos de la empresa.

Para configurar el indicador, especifique hasta dos valores de umbral que definan tres rangos de valores de datos (bajo, medio y alto) a los que se pueda aplicar otro color (o estilo).

## <a name="to-set-up-colored-indicators-on-cues"></a>Para configurar indicadores de color en las pilas
1. En **Actividades** en la página **Inicio**, elija **Configurar pilas**.  
   Aparece la ventana **Configuración de pila**. La ventana muestra los indicadores que están actualmente configurados en pilas.
2. Para modificar un marcador, edite los campos y modifique, por ejemplo, los valores para los distintos umbrales.  

La tabla siguiente muestra los colores que corresponden a las opciones de los campos **Estilo de rango bajo**, **Estilo de rango medio** y **Estilo de rango alto**.

| Opción | Color |
| --- | --- |
| **Ninguno** |Sin color (mismo color que la pila)|
| **Favorable** |Verde |
| **Desfavorable** |Rojo |
| **Ambiguo** |Amarillo |
| **Subordinado** |Gris |

## <a name="see-also"></a>Consulte también
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

