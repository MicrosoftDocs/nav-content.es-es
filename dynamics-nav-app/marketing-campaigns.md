---
title: "Configurar una campaña de marketing en Dynamics NAV"
description: "Describe cómo puede configurar y llevar a cabo campañas de marketing en Dynamics NAV para ayudarle a identificar, atraer y conservar a los clientes."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f8fd64397161f00a289b0d0435ebcf2de76de80
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="managing-marketing-campaigns"></a>Administrar campañas de marketing
Un buen plan de marketing puede permitirle identificar, atraer y conservar a los clientes. Un plan de marketing consta de varias campañas y otras interacciones relacionadas con sus actividades de ventas y marketing. Durante la planificación de una campaña, debe decidir a qué contactos se va a dirigir, el tipo de campaña (por ejemplo, exposición comercial o correo directo) y los vendedores que realizarán las tareas.

Cada campaña consta de diversas actividades o tareas. Puede combinar varias tareas, por ejemplo, tareas que cada una represente un paso, en las actividades. Las tareas de actividad están relacionadas entre sí por medio de una fórmula de fecha. Las tareas individuales solo se pueden asignar a vendedores. Las actividades se pueden asignar a oportunidades, vendedores, grupos de vendedores y contactos. Para obtener más información, vea [Procedimiento: Configurar ciclos y etapas de ciclos de venta de oportunidades](marketing-how-setup-opportunity-sales-cycles-stages.md).

## <a name="defining-individual-campaigns"></a>Definir campañas individuales
Antes de crear una campaña, debe configurar *códigos de estado de campaña*. El uso de estos códigos le permitirá administrar sus campañas asignando un estado a cada una de ellas. A medida que trabaja en las distintas etapas de una campaña, podrá ver en qué etapa de la campaña se encuentra y cuál es el siguiente paso. Los códigos de estado de campaña se configuran en la ventana **Estado campaña**.

Puede crear una ficha de campaña para cada campaña de la que desee realizar un seguimiento. También puede acceder a estas fichas de campañas para ver información general sobre sus campañas.
Puede eliminar los movimientos de campaña, por ejemplo si registran una acción que ha sido cancelada. Sólo se pueden borrar los movimientos de campaña cancelados.

### <a name="selecting-the-target-audience"></a>Selección del público objetivo
Una vez creada una campaña, puede crear segmentos que especifiquen el público objetivo de la campaña. Para obtener más información, vea [Administrar segmentos](marketing-segments.md).

### <a name="registering-discount-percentages"></a>Registrar porcentajes de descuento
Cuando haya configurado su campaña, decidido qué segmentos desea que cubra la campaña y establecido la fecha inicial y final, registre el porcentaje de descuento que recibirá el cliente en cada producto en las líneas de la ventana **Descuentos línea ventas**. También puede registrar precios de venta de los productos individuales en las líneas de la ventana **Precios ventas**. Puede acceder a ambas ventanas desde la ficha de campaña.

 Cuando haya configurado los precios de venta y los descuentos de líneas y los segmentos en la ficha de campaña, debe activarlos para que los precios y descuentos de campaña se reflejen en las líneas.

> [!NOTE]  
>   Para activar los precios de venta y descuentos de línea, debe especificar si todo el segmento o solo algunos contactos son los objetivos de la campaña. Si los precios de venta y descuentos de línea cubren a todos los contactos del segmento, seleccione el campo **Objetivo campaña** de la ficha desplegable **Campaña** de la ficha **Segmento**.

Si los precios de venta y descuentos de línea no se ofrecen a todos los contactos del segmento, puede desactivar el campo **Objetivo campaña** para los contactos relevantes. Si no ve este campo, puede agregarlo a la vista. Para obtener más información, vea [Personalización del usuario](ui-user-personalization.md).

## <a name="conducting-campaigns"></a>Realizar campañas
A medida que se desarrolla una campaña, se registran todas las interacciones con los contactos o segmentos, por lo que puede obtener estadísticas y otra información sobre los costes y los porcentajes de éxito alcanzado.

Las campañas las realizan vendedores y debe crear actividades para representar cada tarea y asignarlas al vendedor relevante. Para obtener más información, vea [Procedimiento: Configurar ciclos y etapas de ciclos de venta de oportunidades](marketing-how-setup-opportunity-sales-cycles-stages.md).

## <a name="see-also"></a>Consulte también
[Gestionar contactos](marketing-contacts.md)  
[Administrar segmentos](marketing-segments.md)  
[Administrar oportunidades de venta](marketing-manage-sales-opportunities.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)  

