---
title: "Métodos WIP para calcular y registrar el progreso del proyecto"
description: "Describe los distintos métodos de trabajo en proceso (WIP) que puede utilizar para registrar, supervisar y calcular la información financiera de los proyectos en curso."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: work in process, work in progress, calculate project WIP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4a472d7a45cacfe4cd2534747f447a1e4ca7a303
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-wip-methods"></a>Comprensión de los métodos WIP
[!INCLUDE[d365fin](includes/d365fin_md.md)] admite los siguientes métodos de cálculo y registro del valor del trabajo en curso.

| Método WIP | Tipo cálculo | Descripción del cálculo |
| --- | --- | --- |
| Valor coste |Ingresos reconocidos = Precio facturado facturable<br /><br /> Total costes estimados = Precio total facturable x Relación coste presupuesto<br /><br /> Costes WIP = (Porcentaje de terminación - % facturado) x Total costes estimados<br /><br /> Porcentaje de terminación = Coste total de uso / Coste total de presupuesto<br /> % facturado = Precio facturado facturable<br /><br /> Costes reconocidos de precio total facturable = Coste total de uso - WIP |Los cálculos del valor del coste se inician calculando el valor de lo que se ha servido tomando una proporción de los costes totales estimados basada en el porcentaje de terminación. Los costes facturados se restan tomando una proporción de los costes totales estimados basada en el porcentaje facturado.<br /><br /> Este cálculo requiere que se hayan introducido correctamente el precio total facturable, el precio total de presupuesto y el coste total de presupuesto para todo el proyecto. |
| Coste de ventas |Ingresos reconocidos = Precio facturado facturable<br /><br /> Costes reconocidos = Coste total de presupuesto x Porcentaje facturado<br /><br /> % facturado = Precio facturado facturable / Precio total facturable<br /><br /> (El % facturado es una columna de las líneas de tarea de proyecto)<br /><br /> Costes WIP = Uso (Coste total) – Costes reconocidos |Los cálculos de los costes de ventas se inician calculando los costes reconocidos. Los costes se reconocen proporcionalmente a partir del coste total de presupuesto.<br /><br /> Este cálculo requiere que se haya especificado correctamente el precio total facturable y el coste total de presupuesto para todo el proyecto. |
| Valor ventas |Costes reconocidos = Uso (Coste total)<br /><br /> Ingresos reconocidos = Uso (Precio total) x Relación facturación esperada<br /><br /> % recuperación coste = Precio total facturable / Precio total de presupuesto<br /><br /> Ventas WIP = Ventas reconocidas - Precio facturado facturable |Los cálculos de valor de ventas reconocen los ingresos proporcionalmente basados en el coste total de uso y la relación de recuperación de costes esperada.<br /><br /> Este cálculo requiere que se haya especificado correctamente el precio total facturable y el precio total de presupuesto para todo el proyecto. |
| Porcentaje de compleción |Costes reconocidos = Uso (Coste total)<br /><br /> Ingresos reconocidos = Precio total facturable x Porcentaje de terminación<br /><br /> Porcentaje de terminación = Coste total de uso / Coste total de presupuesto<br /> (Se denominada "% de terminación del coste" en las líneas de tarea de proyecto)<br /><br /> Ventas WIP = Ventas reconocidas - Precio facturado facturable |Los cálculos de los porcentajes de terminación reconocen los ingresos proporcionalmente a partir del porcentaje de terminación, es decir, el coste total de uso frente al coste de presupuesto.<br /><br /> Este cálculo requiere que se haya especificado correctamente el precio total facturable y el coste total de presupuesto para todo el proyecto. |
| Contrato completado |Importe WIP = Importe coste WIP = Uso (Coste total)<br /><br /> Importe ventas WIP = (Precio facturado) facturable |Contrato consumado no reconoce los ingresos y los costes hasta que haya finalizado el proyecto. Es posible que desee utilizarlo cuando haya gran incertidumbre acerca de las estimaciones en cuanto a costes e ingresos del proyecto.<br /><br /> Todo el consumo se registra en la Cuenta costes WIP (activos) y las ventas facturadas se registran en la Cta. ventas facturadas WIP (pasivos) hasta que el proyecto finalice. |

## <a name="see-also"></a>Consulte también
[Administración de proyectos](projects-manage-projects.md)  
[Finanzas](finance.md)  
[Compras](purchasing-manage-purchasing.md)         
[Ventas](sales-manage-sales.md)      
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

