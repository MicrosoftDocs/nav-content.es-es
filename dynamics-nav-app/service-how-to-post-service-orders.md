---
title: Registrar pedidos de servicio
description: "Una vez que haya creado un pedido de servicio, rellenado toda la información y realizado los cambios necesarios, podrá registrarlo. El pedido debe contener como mínimo una línea de producto de servicio y una línea de servicio para poder registrarlo. Si el pedido contiene más de una línea de servicio, se registrarán todas las líneas de una sola vez."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d93f6520237d2153220654f0f2eb226d8a75adfb
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-service-orders-and-credit-memos"></a>Cómo registrar abonos y órdenes de servicio
Una vez que haya creado un pedido de servicio, rellenado toda la información y realizado los cambios necesarios, podrá registrarlo. El pedido debe contener como mínimo una línea de producto de servicio y una línea de servicio para poder registrarlo. Si el pedido contiene más de una línea de servicio, se registrarán todas las líneas de una sola vez.  

Si tiene un gran número de pedidos de servicio, puede ahorrar mucho tiempo si utiliza un proceso de trabajo por lotes para registrarlos a la vez. Puede ejecutar el trabajo por lotes con cualquier pedido de servicio.

> [!Tip]
> Antes de registrar un documento de servicio, se recomienda que utilice la acción **Informe de prueba** para comprobar los errores o la falta de información. Si hay errores, deberá corregir el problema. Podrá imprimir un nuevo informe de prueba para verificar el fijo y registrar el documento.
  
## <a name="to-post-a-service-order"></a>Para registrar un pedido de servicio    
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el pedido servicio que corresponda.  
3. En la página **Pedido servicio**, seleccione una de las acciones siguientes.  
  
    |**Acción**|**Resultado**|  
    |------------------|----------------|  
    |**Test** | Comprueba todas las partes del documento y muestra el resultado en un informe. Si el informe indica errores o falta de información, deberá solucionar el problema. Una vez solucionado, podrá imprimir un test nuevo.|  
    |**Registrar** | Registra el pedido sin imprimir un albarán o una factura.|  
    |**Registrar e imprimir** | Registra el pedido e imprime un albarán (si se envía el pedido sin facturarlo) o una factura (si se factura el pedido).|  
    |**Registrar por lotes** | Registra los pedidos de servicio múltiples al mismo tiempo una vez.|  
  
4. Cuando se registra el pedido, debe especificar una de las opciones siguientes relacionadas con el modo en que desea registrar el pedido.  
  
    |**Opción de registro**|**Resultado**|  
    |------------------------|----------------|  
    |**Enviar** | Registra el envío de los productos.|  
    |**Factura** | Factura los productos ya enviados.|  
    |**Enviar y facturar** | Factura y envía los productos.|  
    |**Enviar y consumir** | Registra el envío y el consumo del pedido. Actualiza las cantidades correspondientes en las líneas de servicio del pedido y en el documento de envío de servicio registrado previamente.|  
  
Solo puede contabilizar el consumo si la línea contiene una cantidad que se ha enviado pero no se ha facturado ni se ha consumido.  
  
Al registrar el pedido, se crearán los movimientos y los documentos registrados pertinentes. Se actualizarán los campos pertinentes en el documento de pedido de servicio.  

## <a name="to-batch-post-service-orders"></a>Para registrar lotes de pedidos de servicio
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la acción **Registrar por lotes**.  
3.  Puede definir un filtro para seleccionar números de pedido específicos o un intervalo de números de pedido para procesar.  
4.  Elija **Aceptar** para iniciar el trabajo por lotes.  

## <a name="to-post-a-service-credit-memo"></a>Para registrar un abono de servicio  
Cuando haya creado un abono de servicio y lo haya rellenado, podrá registrar el abono. Si hubiese algún error o falta de información en el abono al registrarlo, el proceso se verá interrumpido por un mensaje de error.  
   
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Abonos de servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Cree un abono de servicio nuevo. En la pestaña **Inicio**, en el grupo **Nuevo**, seleccione **Nuevo**.  
3. Rellene los campos necesarios.  
4. En la pestaña **Acciones**, grupo **Registro**, elija **Registrar**. Para imprimir el abono al mismo tiempo que lo registra, seleccione **Registrar e imprimir** en su lugar.  
5. Para probar los abonos antes de registrarlos, seleccione **Test**. Al ejecutar el informe, se verificarán las fechas de registro especificadas en el documento.  
6. Para registrar varios abonos del servicio al mismo tiempo, ejecute el trabajo por lotes **Reg. lotes abonos servicio**. Puede ser una ventaja si tiene que registrar un gran número de abonos.  
  
> [!NOTE]  
>  Es importante especificar toda la información necesaria en los abonos antes de procesarlos. De lo contrario, podrían no registrarse. Cuando el trabajo por lotes finaliza el registro, aparece un mensaje que muestra cuántos abonos de servicio se han registrado.  

## <a name="to-post-consumption-from-a-service-order"></a>Para registrar el consumo de un pedido de servicio  
En el siguiente procedimiento se describe cómo registrar los productos, los costes y/o las horas de recursos empleados para una operación de servicio específica por la que no cobrará al cliente. Tenga en cuenta que puede registrar productos, horas o costes consumidos solamente para un envío registrado que no tenga facturas o consumo registrados.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el pedido de servicio cuyo consumo desee registrar.  
3. Elija el producto de servicio. Elija **Acciones**, elija **Pedido** y, a continuación, elija **Líneas servicio**.  
4. Busque los movimientos requeridos y especifique las cantidades por las que va a registrar un consumo en el campo **Cantidad a consumir**. La cantidad no puede ser superior a la cantidad ya enviada y a la cantidad restante no facturada tras la facturación parcial de este envío.  
  
    > [!NOTE]  
    >  Para registrar el consumo respecto a un proyecto, rellene los campos **Nº proyecto**, **Nº tarea proyecto** y **Tipo línea proyecto** de la línea de servicio.  
  
5. Elija las líneas que desee registrar y, a continuación, seleccione la acción **Registrar**. En la página que se abre, seleccione **Consumo**.  
  
El servicio se registrará como consumido parcial o totalmente, dependiendo del valor del campo **Cantidad a consumir**, y se crearán los movimientos contables relevantes. Asimismo, los documentos de envío de servicio registrados previamente se actualizarán por orden cronológico con las cantidades consumidas. Las cantidades correspondientes se actualizarán en las líneas de servicio del pedido.  

## <a name="to-post-shipments-from-service-orders"></a>Para registrar envíos de pedidos de servicio  
Tras especificar los detalles de un servicio, puede actualizar y registrar las cantidades de productos utilizadas, el tiempo invertido y los costes adquiridos. Como resultado, [!INCLUDE[d365fin](includes/d365fin_md.md)] realiza los cambios necesarios para reflejar el nuevo estado del inventario y el estado actual del procesamiento del pedido específico.  
  
El siguiente procedimiento muestra cómo registrar el envío de artículos de línea de servicio en ubicaciones en las que no se requiera control de almacén.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedido de servicio** y, a continuación, seleccione el vínculo relacionado. 2. En la ventana del pedido de servicio seleccionado, elija **Acciones**, **Pedido**, **Líneas servicio**.  
3. En la ventana **Líneas servicio**, busque los movimientos requeridos y especifique la cantidad que se va a registrar en el campo **Cantidad a enviar**.  
  
   > [!NOTE]  
   >  El valor de la cantidad para enviar depende de si desea registrar el envío total o parcialmente. Si decide enviarlo totalmente, el valor del campo **Cantidad a enviar** debe ser igual que el valor del campo **Cantidad**. Cuando registra un envío parcial, debe especificar la cantidad que desea enviar inicialmente. Si ya ha enviado parte del servicio incluido en el pedido, anote el valor en el campo **Cantidad enviada**. La máxima cantidad que se puede especificar en el campo **Cantidad a enviar** es el número de unidades que aún no se han enviado.  
  
4. Elija **Acciones**, **Registro** y, a continuación, en **Registrar**. En la ventana que aparece, elija **Enviar**.  
  
[!INCLUDE[d365fin](includes/d365fin_md.md)] crea los movimientos (de garantía, de producto, de servicio o de cuenta), genera el documento de envío de servicio registrado y actualiza los campos pertinentes en las líneas de servicio del pedido de servicio.  
  
Si el almacén está configurado para requerir el control de almacén, el envío y el movimiento de los productos de línea de servicio funcionan de la misma forma que para otros documentos de origen. La única diferencia es que los productos de línea de servicio pueden consumirse externa o internamente y por lo tanto requieren dos funciones diferentes de lanzamiento.  
  
Para obtener información acerca de como enviar los productos de línea de servicio en configuraciones avanzadas de almacén, consulte [Picking de los artículos para el envío de almacén](warehouse-pick-items.md).  

## <a name="to-undo-posted-consumption"></a>Para deshacer un consumo registrado  
Puede cancelar el consumo de los pedidos de servicio. Por ejemplo, porque se hayan registrado por error.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Histórico envíos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el envío de servicio registrado cuyo consumo incorrecto se registró.  
3. Elija **Acciones**, seleccione **Envíos** y, a continuación, elija **Líneas de servicio de envíos**.  
4. Seleccione las líneas que contengan el consumo incorrecto y, después, seleccione la acción **Deshacer consumo**.  
  
 Se insertará una línea de envío de servicio de balance con valores negativos en las campos de cantidad de las líneas seleccionadas.  
  
> [!NOTE]  
>  No puede deshacer el consumo del servicio si:  

>    * El pedido de servicio se ha cerrado.  
>    * Se ha registrado el área Proyectos, de modo que hay movimientos del proyecto vinculados.  
  
## <a name="to-post-service-lines"></a>Para registrar líneas de servicio  
Si tiene que trabajar en un pedido de servicio durante un periodo largo de tiempo sin registrarlo, puede que desee registrar algunas de las líneas de servicio vinculadas a éste para, por ejemplo, mantener actualizado el inventario. Para registrar, especifique las cantidades correspondientes en las líneas que se van a registrar. Puede elegir entre registrar las líneas una a una o seleccionar varias líneas a la vez.  
  
El procedimiento siguiente describe el registro del envío directamente de un pedido de servicio en las ubicaciones sin control de almacén configurado. Si la ubicación está configurada para requerir control de almacén, el registro de envío se realiza en otro documento de almacén, dependiendo de la ubicación configurada.
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el pedido de servicio y elija la acción **Líneas de servicio**.  
4. En las líneas que va a registrar, rellene los campos **Cantidad a enviar**, **Cdad. a facturar** y **Cantidad a consumir**, en función del modo en que vaya a registrar las líneas.  
5. Seleccione la acción **Registrar**.
  
## <a name="see-also"></a>Consulte también  
[Registro en la gestión de servicios](service-service-posting.md)  
[Crear un pedido de servicio](service-how-to-create-service-orders.md)  

