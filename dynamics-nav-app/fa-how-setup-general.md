---
title: Configurar activos fijos de contabilidad
description: "Antes de trabajar con activos fijos, debe configurar las cuentas contables predeterminadas, los grupos contables, las claves de asignación, las plantillas y secciones de diario, y los códigos de clase."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ecdb1c85526bf9c2583ed5936c2fcc55a27bcb5d
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-general-fixed-assets-information"></a>Procedimiento: Configurar información general de activos fijos
Para poder gestionar activos fijos, debe configurar las cuentas predeterminadas, las claves de asignación, las plantillas y las secciones del diario que se utilizan para registrar y reclasificar los activos fijos, y clasificar los activos fijos en clases como, por ejemplo, Tangible e Intangible.

## <a name="to-set-up-general-default-values-for-fixed-assets"></a>Para configurar los valores predeterminados generales de los activos fijos
Defina el comportamiento general o la funcionalidad de los activos y configure las series numéricas del documento en la ventana **Configuración de activos fijos**.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Configuración de activos fijos** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-fixed-asset-posting-groups"></a>Para configurar los grupos contables de activos fijos
Puede utilizar grupos de registro para definir los grupos contables de activos fijos. Los movimientos de estos grupos contables se registran en las mismas cuentas contables.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Grupos contables** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la acción **Nuevo**.
3. En la ventana **A/F Ficha grupo contable**, rellene los campos según sea necesario.

    > [!NOTE]  
>   ara asegurarse de que las cuentas de contrapartida de los diferentes registros de activos se insertan automáticamente en las líneas del diario al elegir la acción **Introducir saldo AF**, vaya al siguiente paso que se basa en el registro de apreciación.
4. En la ficha desplegable **Saldo**, en el campo **Cta. contrap. apreciación**, seleccione la cuenta contable en la que desea registrar las contrapartidas para la apreciación.

Para obtener más información sobre cómo usar la acción **Introducir saldo AF** en las líneas del diario general de activos, vea, por ejemplo, [Procedimiento: Revalorizar activos fijos](fa-how-revalue.md).

## <a name="to-set-up-fixed-asset-allocation-keys"></a>Para configurar claves de distribución de activos fijos
Las transacciones pueden distribuirse en varios departamentos y proyectos, según las claves de distribución definidas por el usuario. Por ejemplo, puede configurar una clave de distribución para distribuir los costes de amortización de automóviles con el 35% para el departamento de administración y el 65% para el de ventas. Para obtener más información, consulte [Asignar costes e ingresos](year-allocate-costs-income.md).

Las claves de asignación se aplican a las clases de activos, no a los activos individuales.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Grupos contables** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **A/F Grupos contables**, elija la acción **Distribuciones** y, a continuación, elija un tipo de registro.
3. En la ventana **A/F Distribuciones**, rellene los campos según sea necesario.
4. Repita los pasos 2 y 3 en todos los tipos de registro para los que desea definir claves de distribución.

## <a name="to-set-up-fixed-asset-journal-templates"></a>Para configurar las plantillas del diario de activos
Un libro es un diseño predeterminado de un diario. El libro contiene información de los códigos de seguimiento, informes y números de serie. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).

[!INCLUDE[d365fin](includes/d365fin_md.md)] crea automáticamente una plantilla de diario de activos la primera vez que abre la ventana **Diario de activos**, pero puede configurar plantillas de diario adicionales.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Libros diarios** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario.

## <a name="to-set-up-fixed-asset-journal-batches"></a>Para configurar las secciones del diario de activos
Puede configurar múltiples secciones de diario, que son diarios individuales para cada libro de diario. Por ejemplo, los empleados pueden tener su propia sección de diario que utiliza las iniciales del empleado como nombre de la sección. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Libros diarios** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la plantilla de diario correspondiente y, a continuación, elija la acción **Secciones**.
3. En la ventana **A/F Secciones diario**, rellene los campos según sea necesario.

## <a name="to-set-up-fixed-asset-reclassification-journal-templates"></a>Para configurar las plantillas del diario de reclasificación de activos
Use los diarios de reclasificación dedicados cuando deba transferir, dividir o combinar activos fijos. [!INCLUDE[d365fin](includes/d365fin_md.md)] crea automáticamente una plantilla del diario de reclasificación de activos la primera vez que se abre la ventana **A/F Diario reclasif.**, pero puede configurar plantillas de diarios de reclasificación adicionales. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Libros diarios reclasif.** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario.

## <a name="to-set-up-fixed-asset-reclassification-journal-batches"></a>Para configurar las secciones del diario de reclasificación de activos
Puede configurar múltiples secciones de diario, que son diarios individuales para cada libro de diario reclasificación. Por ejemplo, los empleados pueden tener su propia sección de diario reclasificación que utiliza las iniciales del empleado como nombre de la sección de diario reclasificación. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Libros diarios reclasif.** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la plantilla de diario correspondiente y, a continuación, elija la acción **Secciones**.
3. En la ventana **A/F Secciones diario reclasif.**, rellene los campos según sea necesario.

## <a name="to-set-up-fixed-asset-class-codes"></a>Para configurar códigos de clase de activos
Los códigos de clase de activos fijos se pueden usar para agrupar los activos fijos, por ejemplo, en activos tangibles y activos intangibles.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clases A/F** y, a continuación, seleccione el vínculo relacionado.
2. Especifique los códigos y nombres que desea crear.

## <a name="to-set-up-fixed-asset-subclass-codes"></a>Para configurar códigos de subclase de activos
Puede utilizar los códigos de subclase de activos fijos para agrupar sus activos en las categorías, por ejemplo, edificios, vehículos, mobiliario o maquinaria.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Subclases A/F** y, a continuación, seleccione el vínculo relacionado.
2. Especifique los códigos y nombres que desea crear.

## <a name="to-set-up-fixed-asset-location-codes"></a>Para configurar códigos de ubicación de activos
Puede usar el códigos de almacén A/F para registrar la ubicación del activo, por ejemplo, departamento de ventas, recepción, administración, producción o almacén. Esta información es útil a efectos de seguros e inventario.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ubicaciones A/F** y, a continuación, seleccione el vínculo relacionado.
2. Especifique los códigos y nombres que desea crear para las ubicaciones de activos.

## <a name="to-register-opening-entries"></a>Para registrar movimientos pendientes
Si es la primera vez que utiliza los activos fijos en [!INCLUDE[d365fin](includes/d365fin_md.md)], deberá configurar antes el área de aplicación Contabilidad antes de configurar los activos fijos. La forma de hacerlo depende de si los activos fijos están integrados con la contabilidad.  

 El siguiente procedimiento se utiliza si se van a registrar las transacciones de activos en la contabilidad.  

1. Asegúrese de completar los procedimientos de configuración básica de los activos fijos.  
2. Cree una ficha de activo para cada activo existente.  
3. Configuración de libros depreciación de activos fijos.  
4. Active la integración en contabilidad siguiendo estos pasos.
5. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.  
6. Seleccione la ficha de libro de amortización correspondiente. En la pestaña **Inicio**, grupo **Administrar**, elija **Editar** para abrir la ventana **Ficha libro amortización**.
7. Asegúrese de que todos los campos estén vacíos borrando todas las marcas en la ficha desplegable **Integración**. Si dispone de más de un libro de amortización, active la integración contable de cada uno.  
8. En el diario de activos fijos, introduzca las siguientes líneas por activo:
   * Línea con el coste.
   * Una línea con la amortización acumulada hasta el final del año fiscal anterior.
   * Una línea con la amortización acumulada desde el inicio del año fiscal en curso hasta la fecha en que [!INCLUDE[d365fin](includes/d365fin_md.md)] está establecido para comenzar a calcular la amortización.

Si tiene otros saldos pendientes, también puede especificarlos ahora, como depreciación o apreciación.  

Si los activos fijos no se integran en la contabilidad, omita los pasos del 4 al 7.

## <a name="see-also"></a>Consulte también
[Configurar activos fijos](fa-setup.md)  
[Activos fijos](fa-manage.md)  
[Finanzas](finance.md)  
[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

