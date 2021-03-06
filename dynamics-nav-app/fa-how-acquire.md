---
title: Activos fijos adquiridos
description: "Puede configurar un activo fijo, asignar un libro de amortización y registrar el coste de adquisición del activo fijo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: purchase fixed asset
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 17a61be2cd0977a55b098c8ec0b1d1cc164d7898
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-acquire-fixed-assets"></a>Procedimiento: Adquirir activos fijos
Deberá configurar una ficha con la información de cada activo. Puede configurar los edificios o los bienes de producción como activos principales con una lista de componentes y puede agruparlos de diferentes maneras como, por ejemplo, por clase, departamento o ubicación. Un libro de amortización debe estar configurado y asignado a cada activo fijo antes de que pueda adquirirlo.

Cuando se ha configurado un activo y se le ha asignado un libro de amortización, debe adquirirlo. Para adquirir un activo, registre el coste en la cuenta de contabilidad, la cuenta bancaria o el proveedor correspondiente registrando una transacción de adquisición desde la ventana **A/F Diario general**. Puede utilizar la ventana **Adquisición activos asistida** para crear y registrar las líneas del diario general requeridas automáticamente.

El valor residual es el valor restante de un activo cuando ya no se puede utilizar. Puede registrar el valor residual en el momento de registrar el coste. Para obtener más información, consulte [Procedimiento: Depreciar o amortizar activos fijos](fa-how-depreciate-amortize.md).

El ajuste de valores se utiliza para ajustar los valores a los cambios de niveles generales de precio. El proceso **Ajustar valores activos** puede utilizarse para calcular los costes de adquisición como de sustitución.

## <a name="to-create-a-fixed-asset-and-acquire-it-automatically"></a>Para crear un activo y adquirirlo automáticamente
El procedimiento siguiente describe cómo crear un activo y después adquirirlo utilizando la ventana **Adquisición activos asistida** para crear y registrar las líneas necesarias del diario general de activos. También puede crear y registrar las líneas de diario manualmente. Para obtener más información, consulte la sección "Para registrar una adquisición de un activo manualmente con el diario general de activos".

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Activos fijos** y, a continuación, seleccione el vínculo relacionado.  
2. Elija la acción **Nuevo** y, a continuación, rellene los campos de la ficha desplegable **General** como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. En la ficha desplegable **Ficha libros amortización**, rellene los campos según sea necesario. Este paso asigna un libro de amortización al activo.  
4. Si necesita asignar más de un libro de amortización al activo, elija la acción **Añadir más libros amortización**. Para obtener más información, vea la sección "Para asignar un libro de amortización a un activo" en [Procedimiento: Configurar la amortización de los activos fijos](fa-how-setup-depreciation.md).

    Cuando estén rellenados todos los campos requeridos para adquirir un activo, aparecerá la notificación **Está listo para adquirir el activo. Adquirir** en la parte superior de la página.
5. Seleccione la acción **Adquirir** en la notificación.
6. Siga los pasos de la ventana **Adquisición activos asistida** para completar la adquisición automática del activo.

> [!NOTE]  
>   Puede registrar los costes como abonos. En ese caso, recuerde que el valor del campo **Coste con IVA** debe tener el símbolo menos que indica un abono.

Cuando elige **Finalizar**, se rellena el campo **Valor libro** de la ventana **Ficha activo** e indica que el activo se ha adquirido según el coste especificado.  

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>Para configurar una lista de componentes para un activo principal
Puede agrupar sus activos en principales y sus componentes. Por ejemplo, puede tener un equipo de producción que consista en muchas partes, las cuales desea agrupar de esta manera.  

Tanto el activo principal como todos sus componentes deben configurarse como fichas individuales de activos. Después de configurar una lista de componentes, [!INCLUDE[d365fin](includes/d365fin_md.md)] rellena automáticamente los campos **Principal/Componente** y **Componentes de activo principal** de las fichas de activos fijos.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Activos fijos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo principal y, a continuación, elija la acción **Componentes activo ppal**.
3. En la ventana **Componentes activo ppal.**, seleccione el campo **A/F Nº** y, a continuación, seleccione el activo que desea agregar como componente del activo principal.
4. Cierre la ventana.
5. Repita los pasos 3 y 4 para cada componente que desee agregar.
6. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Configuración de activos fijos** y, a continuación, seleccione el vínculo relacionado.
7. Seleccione la casilla de verificación **Permitir reg. en activos pples**.

## <a name="to-post-a-fixed-asset-acquisition-manually-with-the-fixed-asset-gl-journal"></a>Para registrar una adquisición de activo manualmente con el diario general de activos fijos
El procedimiento siguiente describe cómo adquirir un activo manualmente creando y registrando líneas en la ventana **A/F Diario general**. También puede adquirir un activo de manera automática utilizando la ventana **Adquisición activos asistida**. Para obtener más información, consulte el paso 5 en la sección "Para crear un activo y adquirirlo automáticamente".

> [!NOTE]  
>   Puede registrar los costes como abonos. En ese caso, recuerde que el valor del campo **Importe** debe tener el símbolo menos que indica un abono.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **A/F Diario general**, en el campo **A/F Tipo registro**, seleccione **Coste**.
3. Rellene los campos restantes según sea necesario.
4. Seleccione la acción **Registrar**.  

> [!TIP]  
>   Si rellena el campo **Nº seguro** del diario general de activos fijos en el momento de registrar un coste, [!INCLUDE[d365fin](includes/d365fin_md.md)] también registrará el coste del activo en los movimientos de seguros. Para obtener más información, vea [Procedimiento: Asegurar activos fijos](fa-how-insure.md).

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>Para anular un coste del registro de un activo
Si se equivoca al registrar un coste, puede eliminar el movimiento mediante el proceso **Cancelar movs. A/F** y registrar seguidamente el movimiento de adquisición correcto. Los movimientos incorrectos se transfieren a la ventana **A/F Movs. anulados**.

Por ejemplo, si registra una adquisición con la fecha incorrecta, debe corregirla lo más pronto posible porque la fecha de registro de un activo se utiliza para realizar muchos cálculos importantes.

> [!IMPORTANT]  
>   No puede usar la función **Transacciones inversas** para los movimientos de un activo.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cancelar movs. A/F** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Elija el botón **Aceptar** para iniciar el trabajo por lotes.
4. Cuando se hayan cancelado el movimiento o movimientos incorrectos, registre el coste correcto.

Para anular los movimientos de varios activos fijos a la vez, use el proceso **A/F Anular movs**.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>Para registrar el valor residual junto con el coste
Puede registrar el valor residual junto con el coste a partir del diario general de activos.    

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cancelar movs. A/F** y, a continuación, seleccione el vínculo relacionado.
2. Cree la línea de adquisición del diario. Para obtener más información, consulte la sección "Para registrar una adquisición de un activo manualmente con el diario general de activos".
3. En el campo **Valor residual** de la línea del diario, escriba el importe del valor residual como abono (con un signo menos).
4. Seleccione la acción **Registrar**.

> [!NOTE]  
>   El tipo de registro **Valor residual** es una opción exclusiva de la ventana **Diario de activos**. No está disponible en la ventana **A/F Diario general** porque el valor residual nunca se registra en el libro mayor.

## <a name="see-also"></a>Consulte también
[Activos fijos](fa-manage.md)  
[Configurar activos fijos](fa-setup.md)  
[Finanzas](finance.md)  
[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

