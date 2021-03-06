---
title: "Crear una ubicación desde la ubicación interna"
description: "Una vez ubicados los productos y antes de que se realice el picking de los mismos para cubrir las necesidades de una orden de producción o un envío, los productos se almacenan en el almacén como parte de las existencias disponibles."
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
ms.openlocfilehash: 970b9b9046018b0dcea5b9996d10e19e444a7639
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-pick-and-put-away-without-a-source-document"></a>Realizar el picking y la ubicación sin un documento de origen
Una vez ubicados los productos y antes de que se realice el picking de los mismos para cubrir las necesidades de una orden de producción o un envío, los productos se almacenan en el almacén como parte de las existencias disponibles.  

Puede darse el caso de que haya que sacar productos de las ubicaciones de picking de almacén temporalmente para utilizarlos como modelos de demostración en una presentación de ventas. Estos productos pertenecen a la empresa y forman parte de las existencias, pero no están disponibles para picking. Se registran en una ubicación especial que se crea con este fin; técnicamente, los productos están en el almacén, pero físicamente estarían en una sala de demostraciones.  

En otras situaciones, el departamento de producción es posible que necesite, de forma inesperada, determinados componentes para su proceso. Puede realizar el picking de productos para las ubicaciones de producción con un picking interno. Cuando finalice el proceso y se cree la salida, registre el consumo de los productos y vacíe la ubicación de producción, lo que reducirá la cantidad del producto en su almacén.  

De igual modo, los productos se pueden devolver al almacén para ubicarlos. Puede que los productos se hayan pasado del inventario disponible a una orden de producción y no se hayan utilizado. Deben ubicarse en el almacén para que formen parte de nuevo del inventario disponible.  

Los **Picking internos** le permiten realizar ubicaciones sin tener que hacer referencia a un documento de origen determinado. Puede configurar fácilmente toda la información que necesita para crear una instrucción de almacén de ubicación.  

> [!NOTE]  
>  Si no utiliza ubicación y picking directos, estos ajustes se pueden realizar con los métodos para mover productos entre ubicaciones o registrar ajustes de cantidades en una ubicación.  
>   
>  Cuando el almacén utiliza ubicación y picking directos y, por tanto, utiliza tipos de ubicaciones, no puede mover manualmente productos dentro o fuera de una ubicación de tipo RECEPCIÓN, porque los productos que están en una ubicación de tipo RECEPCIÓN deben ubicarse antes de que formen parte del inventario disponible.  

## <a name="to-create-an-internal-pick"></a>Para crear un picking interno  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Picking interno almacén** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene el campo **No.**. y **Hasta cód. ubicación** de la ficha desplegable **General**. El campo **Hasta cód. ubicación** especifica la ubicación desde la que desea traer los productos. Para producción, esta ubicación sería la ubicación de producción de entrada o la ubicación de planta abierta. Para otros fines, seleccione un Hasta cód. ubicación de tipo ubicación que no se utilice para picking, probablemente una ubicación especial, de envío o intermedia.  
3.  Seleccione un producto en el campo **Nº producto** y rellene las cantidades que desea realizar el picking.  
4. Elija la acción **Crear picking**. Ahora está preparada una instrucción de picking de almacén para que un empelado la ejecute.  

## <a name="to-create-an-internal-put-away"></a>Para crear un ubicación interna  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ubicación interna almacén** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene el campo **No.**. y **Desde cód. ubicación** de la ficha desplegable **General**. El campo **Desde cód. ubicación** especifica la ubicación donde se encuentran los productos devueltos al almacén, probablemente de producción.  
3.  Rellene los números y las cantidades de productos de las líneas.  
4.  Seleccione la acción **Crear ubicación**. Ahora está preparada una instrucción de ubicación de almacén para que un empelado la ejecute.  

## <a name="see-also"></a>Consulte también  
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

