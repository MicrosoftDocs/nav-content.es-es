---
title: "Configurar procesos de producción"
description: "Para convertir material en artículos producidos finales, se deben configurar recursos de producción, como listas de materiales, ruta, operadores de máquina y maquinaria, en el sistema."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b22fe53cc9a9ce6bb357f9eaf54fc37c4e1242b9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-manufacturing"></a>Configuración de fabricación
Para convertir material en artículos producidos finales, se deben configurar recursos de producción, como listas de materiales, ruta, operadores de máquina y maquinaria, en el sistema.

Los operadores y máquinas se representan en el sistema como centros de máquina que pueden organizarse en centros de trabajo y grupos de centros de trabajo. Cuando se establecen estos recursos, se pueden cargar con operaciones, en función de la estructura del proceso (ruta) y el material definido (L.M.) para el artículo y en función de la capacidad del centro de trabajo o de máquina. También se puede definir la capacidad de producción de cada recurso. La capacidad se define según el tiempo de trabajo disponible en los centros de trabajo y de máquina y se controla mediante calendarios para cada nivel. El calendario de un centro de trabajo especifica los días u horas laborales, turnos, vacaciones y ausencias que determinan la capacidad bruta disponible del centro de trabajo (normalmente, se mide en minutos). Todo esto se determina a partir de valores de capacidad y eficiencia definidos.  

Cuando haya configurado la fabricación, puede planificar y ejecutar las órdenes de producción. Si desea obtener más información, consulte [Planificación ](production-planning.md) y [Fabricación](production-manage-manufacturing.md).  

 En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.   

|**Para**|**Vea**|  
|------------|-------------|  
|Configurar las características de fabricación, como la definición de las horas laborales de la planta y la selección de principios de planificación.|La página **Configuración de fabricación**.|  
|Definir una semana laboral estándar, en el departamento de fabricación, en términos de horas de inicio y fin de cada día laboral y turno de trabajo relacionado.|[Cómo crear calendarios de planta](production-how-to-create-work-center-calendars.md)|  
|Organizar valores fijos y requisitos de un recursos de producción, como centros de trabajo o centros de máquinas, para controlar la salida de la producción efectuada.|[Procedimiento: Configuración de centros de trabajo y centros de máquinas](production-how-to-set-up-work-and-machine-centers.md)|
|Organizar las operaciones de producción en la orden requerida y asignarlas a los centros de trabajo o centros de máquinas con los horarios de trabajo necesarios.|[Creación de rutas](production-how-to-create-routings.md)|
|Organizar componentes o subconjuntos de producción sujetos a un producto principal producido y certificar la L.M. para la ejecución en los centros de trabajo.|[Creación de L.M. de producción](production-how-to-create-production-boms.md)|
|Asegúrese de que la cantidad correcta de componentes están disponibles cuando los artículos producidos se almacenan en una unidad de medida pero se produjeron en otra.|[Procedimiento: Trabajar con la unidad de medida de lote de fabricación](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)|  
|Definir familias de artículos de producción con procesos de fabricación similares para ahorrar consumo. Por ejemplo, se pueden fabricar cuatro piezas de un mismo producto desde una hoja y 10 piezas de otro producto distinto al mismo tiempo.|[Procedimiento: Trabajo con familias de producción](production-how-work-family.md)|
|Uso de tareas estándar para simplificar la creación de rutas adjuntando rápidamente información adicional a operaciones periódicas.|[Cómo configurar de líneas de ruta estándar](production-how-set-up-standard-routing-lines.md)|  
|Prepare centros de trabajo y rutas para representar operaciones de producción subcontratadas.|[Procedimiento: Subcontratación de fabricación](production-how-to-subcontract-manufacturing.md)|  

## <a name="see-also"></a>Consulte también
[Fabricación](production-manage-manufacturing.md)    
[Planificación](production-planning.md)   
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

