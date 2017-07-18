---
title: 'Procedimiento: Mantener activos fijos'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 58077a38433a73b981a6f3d05ce7ed106acf32f4
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-maintain-fixed-assets"></a>Procedimiento: Mantener activos fijos
Los gastos de mantenimiento son costes periódicos habituales necesarios para mantener el valor de los activos fijos. A diferencia de los incrementos de capital, estos no aumentan de valor.

Puede registrar y mantener un archivo actualizado del mantenimiento y servicio de sus activos fijos para tener registros de mantenimiento completos en un activo fácilmente accesible. Cada vez que se envía un activo a recibir servicio se registran todos los datos importantes, como la fecha de servicio, el número de proveedor y el número de teléfono del agente de servicio. El registro de mantenimiento se realiza para cada activo desde la ficha de activos fijos pertinente.

El ajuste de valores se utiliza para ajustar los valores a los cambios de niveles generales de precio. El proceso **Ajustar valores activos** puede utilizarse para volver a calcular los costes de mantenimiento.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>Para registrar el trabajo de mantenimiento en un activo  
Cada vez que se realiza mantenimiento, como un servicio de visita, puede registrarlo en el activo correspondiente en la ventana **Registros mantenimiento**.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione el activo en el que desea registrar el mantenimiento y, a continuación, elija la acción **Registro mantenimiento**.
3. En la ventana **Registro mantenimiento**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>Para registrar los costes de mantenimiento a partir de un diario general de activos fijos
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Lista libros amortización** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione el libro de amortización que se ha asignado al activo y, a continuación, elija la acción **Editar**.
3. En la ventana **Ficha libro amortización**, asegúrese de que la casilla **Mantenimiento** no está seleccionada. Esto asegura que los costes de mantenimiento no se registren en el libro mayor.
4. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.  
5. Cree una línea inicial de diario y rellene los campos según sea necesario.
6. En el campo **A/F Tipo registro**, seleccione **Mantenimiento**.
7. Elija la acción **Introducir saldo AF**. Se crea una segunda línea de diario para la cuenta contrapartida que se ha configurado para el registro de mantenimiento.

    **Nota**: El paso 7 solo funciona si ha configurado lo siguiente: en la ventana **A/F Ficha grupo contable** del grupo contable del activo fijo, el campo **Cta. mantenimiento** contiene la cuenta de cargo y el campo **Cta. contrap. mantenimiento** contiene la cuenta contable en la que desea registrar los movimientos de contrapartida para apreciación. Para obtener más información, vea la sección "Para configurar grupos contables de activos fijos" en [Procedimiento: Configurar información general del activo fijo](fa-how-setup-general.md).
8. Seleccione la acción **Registrar**.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>Para realizar un seguimiento de visitas servicio en activos fijos
Puede imprimir el informe **Mnto. - Próxima revisión** para ver los activos programados con una visita. Puede utilizar este informe en el momento de actualizar el campo **Próxima fecha servicio** en las fiches de activos fijos.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Próxima revisión mantenimiento** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos **Fecha inicial** y **Fecha final**  
3. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="to-monitor-maintenance-costs"></a>Para supervisar costes de mantenimiento  
Puede ver los costes de mantenimiento si consulta las estadísticas de un activo.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo en el que desea ver los costes de mantenimiento y, a continuación, elija la acción **Libros amortización**.
3. En la ventana **Libros amortización A/F**, seleccione el libro de amortización de activos correspondiente y, a continuación, elija la acción **Estadísticas**.
4. En la ventana **Estadísticas activos fijos**, elija el campo **Mantenimiento**.

La ventana **Movs. mantenimiento** se abre y muestra los movimientos que conforman el importe en el campo **Mantenimiento**.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>Para ver o imprimir los costes de mantenimiento de varios activos fijos  
En el informe **Mnto. - Análisis**, puede seleccionar la vista de mantenimiento según uno, dos o tres códigos de mantenimiento para una fecha o periodo especificados. Puede ver el total de los activos seleccionados o un total para cada uno.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Análisis mantenimiento** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.
3. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="to-view-maintenance-ledger-entries"></a>Para ver movimientos de mantenimiento
Puede estudiar también los costes de mantenimiento si consulta los movimientos en el libro mayor.  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo en el que desea ver los movimientos de contabilidad y, a continuación, elija la acción **Libros amortización**.
3. En la ventana **Libros amortización A/F**, seleccione el libro de amortización de activos correspondiente y, a continuación, elija la acción **Movs. mantenimiento**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>Para ver o imprimir los movimientos de mantenimiento de varios activos fijos  
En el informe **Mnto. - Detalles**, puede ver o imprimir los movimientos de mantenimiento para uno o varios activos fijos.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Detalles mantenimiento** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.
3. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

