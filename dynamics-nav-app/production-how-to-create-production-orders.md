---
title: "Creación de cabeceras de orden de producción"
description: "Puede crear una orden de producción manualmente y el primer paso es crear la cabecera."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 653451206fe0baec63e9db4cce7626357bb00942
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-production-order-headers"></a>Creación de cabeceras de orden de producción
Puede crear una orden de producción manualmente y el primer paso es crear la cabecera.

Las órdenes de producción normalmente se crean automáticamente por algunas tareas de planificación para cubrir una demanda conocida. Para obtener más información, consulte [Planificación](production-planning.md).   

En el siguiente procedimiento, se crea una orden de producción planificada en firme. Puede también crear órdenes de producción con estados distintos.  

## <a name="to-create-a-production-order-header"></a>Para crear la cabecera de una orden de producción  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **O.P. Planificadas en firme** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3.  En el campo **N.º**, inserte el número siguiente de la serie.  
4.  En el campo **Tipo procedencia mov.**, seleccione la procedencia del movimiento de la orden de producción.

    Aquí puede seleccionar producir para una familia de productos. Para obtener más información, consulte [Cómo trabajar con familias de producción](production-how-work-family.md).
5.  En el campo **Cód. procedencia mov.**, seleccione el código de producto, familia o cabecera de venta para el cual se va a generar la orden de producción.  
6.  Rellene los campos **Cantidad** y **Fecha vencimiento** según sus especificaciones.  

Cuando cambian las necesidades de producción, como componentes u operaciones, puede replantear rápidamente la orden de producción. Para obtener más información, vea [Procedimiento: Replanificar o actualizar las órdenes de producción directamente](production-how-to-replan-refresh-production-orders.md). 

## <a name="see-also"></a>Consulte también  
[Fabricación](production-manage-manufacturing.md)    
[Configuración de fabricación](production-configure-production-processes.md)  
[Planificación](production-planning.md)      
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

