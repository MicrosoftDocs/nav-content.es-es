---
title: Crear una ficha de proveedor para registrar un proveedor nuevo
description: "Obtenga información sobre cómo crear una ficha de proveedor para registrar un nuevo proveedor."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c7fee8b43940fc5e5fb020b4ca1ac9b27b90decd
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-new-vendors"></a>Registro de proveedores nuevos
Los proveedores proporcionan los productos que vende. Cada proveedor del que compra debe estar registrado como ficha de proveedor.

Antes de que pueda registrar nuevos proveedores, debe configurar varios códigos de compra que pueda seleccionar al rellenar fichas de proveedores. Una vez creados todos los datos maestros necesarios, se puede efectuar una configuración adicional del proveedor, como priorizar el proveedor para fines de pago y crear una lista de productos que este y otros proveedores pueden suministrar. Otro grupo de tareas de configuración para proveedores es registrar los acuerdos relativos a descuentos, precios y métodos de pago. Para obtener más información, consulte [Configurar compras](purchasing-setup-purchasing.md).

Las fichas de proveedor contienen la información necesaria para comprar productos del proveedor. Para obtener más información, vea [Registrar compras](purchasing-how-record-purchases.md) y [Registrar nuevos productos](inventory-how-register-new-items.md).

> [!NOTE]  
>   Si existen plantillas de proveedor para distintos tipos de proveedor, una ventana aparece cuando se crea una nueva ficha de proveedor en la que puede seleccionar una plantilla adecuada. Si solo existe una plantilla de proveedor, las nuevas fichas de proveedor utilizan siempre esa plantilla.

## <a name="to-create-a-new-vendor-card"></a>Para crear una nueva ficha de proveedor
1. En la página Inicio, seleccione **Proveedores** para abrir la lista de fichas de proveedores existentes.  
2. En la ventana **Proveedores**, seleccione **Nuevo**.

    Si existe más de una plantilla de proveedor, se abre una ventana desde la que puede seleccionar una plantilla de proveedor. En ese caso, siga los dos pasos siguientes.
3. En la ventana **Seleccionar una plantilla para un proveedor nuevo**, seleccione la plantilla que quiere usar para la nueva ficha de proveedor.
4. Elija el botón **Aceptar**. Una nueva ficha de proveedor se abre con algunos campos completados con la información de la plantilla.
5. Empiece a rellenar o cambiar campos en la ficha de proveedor, según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Si no conoce de antemano la dirección de facturación que se utilizará para todas las facturas de un proveedor, no rellene el campo **Pago a-Nº proveedor** de la ficha de proveedor. En su lugar, elija el número del pago-a proveedor cuando haya configurado una oferta, pedido o encabezado de compra.

El proveedor estará registrado y la ficha de proveedor está lista para usarse en los documentos de compra.

Si desea usar esta ficha de proveedor como plantilla cuando cree nuevas fichas de proveedor, puede guardarla. Para obtener más información, vea la siguiente sección:

## <a name="to-save-the-vendor-card-as-a-template"></a>Para guardar la ficha de proveedor como una plantilla
1. En la ventana **Ficha de proveedor**, seleccione la acción **Guardar como plantilla**. La ventana **Plantilla proveedor** se abre mostrando la ficha de proveedor como plantilla.
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Para volver a usar dimensiones en las plantillas, seleccione la acción **Dimensiones**. La ventana **Plantilla de dimensiones** se abre mostrando los códigos de dimensión configurados para el proveedor.
4. Modifique o introduzca los códigos de dimensión que se aplicarán a nuevas fichas de proveedor creadas con la plantilla.
5. Cuando haya finalizado la nueva plantilla de proveedor, seleccione el botón de **Aceptar**.  
   La plantilla de proveedor se agrega a la lista de plantillas de proveedor, de modo que puede usarla para crear nuevas fichas de proveedor.

## <a name="see-also"></a>Consulte también
[Compras](purchasing-manage-purchasing.md)  
[Registro de compras](purchasing-how-record-purchases.md)   
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

