---
title: Comprar productos o servicios para un proyecto y administrar suministros
description: "Describe cómo administrar el suministro y la compra de materiales y de servicios para los proyectos."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3405af0c06df0fb04c528cf114d4ef6326f7c0a9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-job-supplies"></a>Administración de suministros de proyecto
La administración de los suministros de los productos, servicios y gastos de un proyecto es un aspecto clave y fundamental de la ejecución de todos los proyectos. Puede utilizar las cantidades de inventario o realizar compras de proyecto mediante pedidos de compra o facturas de compra. Por ejemplo, un proyecto de servicio en un equipo precisa un disco nuevo. Debe crear una factura de compra para comprar un disco nuevo y registrar el proyecto en el que se va a usar.

Si el proceso de compra no requiere que la transacción física de registre por separado, se puede procesar una compra en la ventana **Diario general proyecto**. Para obtener más información, consulte [Registro del uso para proyectos](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Para comprar productos o servicios para un proyecto
El siguiente procedimiento muestra cómo utilizar una factura de compra para comprar productos de un proyecto. Los mismos pasos se aplican al utilizar un pedido de compra.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas compra** y, a continuación, seleccione el vínculo relacionado.  
2. Elija la acción **Nuevo** y, a continuación, rellene los campos según sea necesario. Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).
3. En los campos **Nº proyecto** y **N.º tarea de trabajo**, seleccione la información del proyecto para el que desea comprar productos o servicios. Use la función **Elegir columnas** si el campo no está visible. Para obtener más información, vea [Personalización del usuario](ui-user-personalization.md).

    El valor que seleccione en el campo **Tipo línea proyecto** define si una línea de planificación se crea cuando registra el uso del producto. Si el campo contiene **Facturable**, se crean las líneas de planificación de proyecto preparadas para facturarlas al cliente. Para obtener más información, vea [Facturación de proyectos](projects-how-invoice-jobs.md).
4. Seleccione la acción **Registrar**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Para ver el valor de compras de un proyecto
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Proyectos** y, a continuación, seleccione el vínculo relacionado.
2. Abra una ficha de un proyecto relevante.

    En la ficha desplegable **Tareas**, el campo **Pedidos pendientes** muestra el importe total de los pedidos en divisa local, los productos y servicios de inventario en los documentos de compras de la línea de tarea de proyecto.  

    El campo **Importe recibido no facturado** muestra el valor de los productos entregados en un documento de compra pero que no están facturados.  
3. Seleccione cualquier de los campos para abrir la ventana **Líns. compra** donde puede revisar la información sobre las líneas de documento de compra, incluyendo qué productos o servicios se han recibido.

## <a name="to-post-a-job-related-expense"></a>Para registrar un gasto relacionado con el proyecto
Si tiene costes de proyecto extraordinarios o únicos, puede utilizar la ventana **Diario general proyecto** para enviarlos directamente a la cuenta de proyecto relevante.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios generales proyecto** y, a continuación, seleccione el vínculo relacionado.  
2. Cree una línea nueva y especifique los datos del gasto, incluidos los campos **Nº proyecto** y **Nº tarea proyecto**.  
3. Cuando el diario esté completo, seleccione la acción **Registrar**.

## <a name="see-also"></a>Consulte también
[Administración de proyectos](projects-manage-projects.md)  
[Finanzas](finance.md)  
[Compras](purchasing-manage-purchasing.md)         
[Ventas](sales-manage-sales.md)      
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

