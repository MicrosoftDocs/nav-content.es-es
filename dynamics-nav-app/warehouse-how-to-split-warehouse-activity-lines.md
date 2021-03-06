---
title: "Procedimiento: divida las líneas de actividad de almacén"
description: "En ubicaciones, movimientos o picking de almacén y en ubicaciones y picking de inventario, se sugieren las ubicaciones para el picking o la ubicación de productos. La cantidad real de la ubicación sugerida quizá no sea suficiente, o no hay sitio suficiente en la ubicación sugerida para ubicar la cantidad requerida. En estos casos, necesita dividir la línea para que los productos de esa línea se obtengan o coloquen en varias ubicaciones."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d113b83d2c4d21463e1a015e7015bc1f566652f9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-split-warehouse-activity-lines"></a>Procedimiento: divida las líneas de actividad de almacén
En ubicaciones, movimientos o picking de almacén y en ubicaciones y picking de inventario, se sugieren las ubicaciones para el picking o la ubicación de productos. La cantidad real de la ubicación sugerida quizá no sea suficiente, o no hay sitio suficiente en la ubicación sugerida para ubicar la cantidad requerida. En estos casos, necesita dividir la línea para que los productos de esa línea se obtengan o coloquen en varias ubicaciones.  

El procedimiento siguiente se aplica a todos los documentos de almacén, como ubicación de almacén, movimiento y las líneas de picking, o la ubicación de inventario, movimiento y líneas de picking.  

## <a name="to-split-warehouse-activity-lines"></a>Para dividir líneas de actividad de almacén  
1.  Abra una línea de actividad de almacén en donde esté intentando gestionar una cantidad insuficiente.  
2.  En el campo de **Cdad. a manipular**, introduzca la cantidad reducida que pueda manipular.  
3.  En la ficha desplegable **Líneas**, elija **Acciones**, **Funciones** y **Dividir línea**. Aparecerá una nueva línea, que es una copia de la línea original, excepto en que el campo **Cdad. a manipular** contiene la cantidad que ha eliminado de la línea original.  
4.  Asigne una ubicación adecuada y, si utiliza ubicación y picking directos, una zona, a esta nueva línea, o continúe dividiendo la línea según sea necesario hasta que encuentre ubicaciones apropiadas para toda la cantidad.  

> [!NOTE]  
>  Si utiliza ubicación y picking directos y divide las líneas, debe estar familiarizado con el almacén y poder elegir una ubicación que cumpla los requisitos de almacenamiento del producto y cubra los requisitos generales del documento de almacén. Por ejemplo, no debería dividir una línea de un documento de picking y colocar algunos productos en el área de almacenamiento masivo.  

## <a name="see-also"></a>Consulte también  
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

