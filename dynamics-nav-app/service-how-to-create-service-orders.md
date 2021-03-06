---
title: Crear pedidos de servicio
description: "Puede utilizar la ventana **Pedido servicio** para crear documentos en los que se introduce información acerca de un servicio, como reparación y mantenimiento, de productos de servicio a solicitud del cliente."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: aa0578c7311fcd997653c6dc6d31325abd1d367c
ms.contentlocale: es-es
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-service-orders"></a>Cómo crear pedidos de servicio
Puede utilizar la ventana **Pedido servicio** para crear documentos en los que se introduce información acerca de un servicio, como reparación y mantenimiento, de productos de servicio a solicitud del cliente.  
  
Cuando cree un pedido de servicio, solo tendrá que rellenar algunos campos. Algunos campos son opcionales y muchos se rellenarán automáticamente cuando rellene los campos correspondientes.  
  
## <a name="to-create-a-service-order"></a>Para crear un pedido de servicio    
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Cree un pedido de servicio nuevo.  
3. En el campo **N.º**, introduzca un número para el pedido de servicio.  
  
     Si ha configurado números de serie para pedidos de servicio en la ventana **Config. gestión servicio**, también puede presionar Enter para seleccionar el siguiente número de pedido de servicio disponible.  
  
4. En el campo **Nº cliente**, seleccione el cliente pertinente de la lista. Los campos correspondientes al cliente se rellenan con información de la tabla **Cliente**.  
  
5. Dependiendo de la configuración de la ficha desplegable **Campos obligatorios** de la ventana **Configurar gestión servicios**, puede que necesite rellenar el campo **Tipo pedido de servicio** y el campo **Código de vendedor**.  
6. Si lo desea, puede rellenar el resto de los campos.  
7. Registre las líneas de producto de servicio.  

## <a name="to-create-a-service-order-from-a-contract"></a>Para crear un pedido de servicio a partir de un contrato  
Puede basarse en contratos de servicio para crear automáticamente ofertas de servicio de mantenimiento de productos de servicio.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Crear pedidos serv. contrato** y, a continuación, elija el vínculo relacionado.  
2. Defina los filtros que desea aplicar en la ficha desplegable **Cabecera contrato servicio**.  
3. En la ficha desplegable **Opciones**, rellene los campos **Fecha inicial** y **Fecha final** con la fecha inicial y final del periodo para el que desee crear pedidos de servicio de contratos. El proceso crea ofertas de servicio que incluyen productos de servicio de contratos de servicio con las siguientes fechas de servicio planificadas dentro de este periodo.  
  
    > [!NOTE]  
    >  Existe un límite en el número de días que puede utilizar como rango de fechas cada vez que se ejecuta el trabajo por lotes. Este límite se establece en el campo **Días máx. ped. serv. contrato** de la ventana **Config. gestión servicio**.  
  
4. En el campo **Acción**, seleccione **Crear pedido servicio**.  

## <a name="to-convert-a-service-quote-to-a-service-order"></a>Para convertir una oferta de servicio en un pedido de servicio
Una vez que el cliente ha aceptado la oferta de servicio, puede convertirla en un pedido de servicio. La oferta se elimina y se configura un nuevo pedido de servicio con la misma descripción que la oferta de servicio. Se vuelven a calcular la fecha y el tiempo de respuesta del pedido de servicio y el estado se establece como **Pendiente**. El estado de reparación de los productos de servicio del pedido se cambian a **Inicial**.  
  
[!INCLUDE[d365fin](includes/d365fin_md.md)] busca movimientos de asignación para todos los productos de servicio de la oferta de servicio cuyo estado sea **Activo**. Si encuentra los movimientos de asignación, se actualiza su estado de asignación a **Reasignación necesaria**. Cuando se reasignan los productos de servicio del pedido de servicio, se actualiza el estado de los movimientos de asignación registrados para la oferta a **Terminado**.   

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ofertas de contrato de servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Elija la oferta de servicio relevante que desee convertir en pedido de servicio.  
3. Seleccione la acción **Crear pedido**.  

## <a name="to-check-item-availability-for-one-or-more-orders"></a>Comprobación de la disponibilidad de los artículos para uno o varios pedidos de servicio  
Es posible comprobar si el artículo necesario para cubrir un pedido está en existencias y, en caso contrario, averiguar cuándo lo estará. Además, si es posible efectuar la reserva de un artículo, podrá reservarlo para asegurarse de que esté disponible para el uso. Puede activar la disponibilidad de un pedido determinado o de todos los pedidos.  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Panel despacho** y, a continuación, seleccione el vínculo relacionado.  
2. Realice una de las siguientes acciones:  
  
    * Para un pedido determinado, selecciónelo y, a continuación, elija la acción **Panorama de demanda**.  
    * En todos los pedidos, elija **Mostrar documento**. Se abre la ventana **Pedido servicio**.  
  
3. En la página **Panorama de demanda**, expanda el grupo de productos, y consulte la información acerca de la disponibilidad del producto. Por ejemplo, puede ver cuántos productos están en el inventario. También puede ver cuando un artículo estará disponible si se trata de un pedido pendiente, es decir, cuando el tipo de origen = compra o si se ha reservado. 

## <a name="to-reserve-an-item-for-a-service-order"></a>Reservar un artículo para un pedido de servicio
Si necesita asegurarse de que un producto está disponible para el pedido de servicio, puede reservarlo. 

1. En el cuadro **Buscar**, escriba **Pedidos de servicio** y, a continuación, elija el vínculo relacionado.  
2. Elija la orden de servicio y, a continuación, **Editar**.  
3. Elija **Acciones**, elija **Pedido** y, a continuación, elija **Líneas servicio**.  
4. En la página **Líneas servicio**, seleccione el producto para reservar y, a continuación, elija la acción **Reserva**.  
5. En la página **Reservas**, elija **Reservar desde línea actual**. 

## <a name="to-insert-lines-based-on-standard-service-codes"></a>Para insertar líneas basadas en el servicio estándar  
Si ha configurado códigos de servicio estándar y los ha asignado a grupos de productos de servicio, puede insertar las líneas estándar vinculadas a los códigos de servicio estándar en documentos de servicio. Para obtener más información, consulte [Cómo configurar códigos de servicio estándar](service-how-setup-service-coding.md).   

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Cree un pedido de servicio nuevo.  
3. Rellene los campos según sea necesario.  
4. Rellene las líneas de producto de servicio con la información requerida.  
5. Elija la línea con el artículo de servicio para el que desea crear las líneas de servicio y elija **Traer cód. servicio estánd**. Se abrirá la ventana **Códs. grupo prod. serv. est.** con los códigos estándar para el grupo de artículo de servicio especificado en la línea.  
6. Elija el código adecuado y haga clic en **Aceptar** para insertar líneas de servicio estándar.  
  
> [!NOTE]  
>  Si el campo **Cód. grupo prod. servicio** de la línea de artículo de servicio del documento está en blanco, quiere decir que el artículo de servicio no pertenece a ningún grupo de artículo de servicio. En este caso, la ventana **Códs. grupo prod. serv. est.** contendrá una lista de todos los códigos de servicio estándar. Debe seleccionar las líneas de la lista para insertar líneas de servicio estándar en el documento. También puede seleccionar de la lista de códigos de servicio estándar asignados a un grupo específico de artículos de servicio. Para ver la lista, seleccione el código correspondiente en el campo **Cód. grupo prod. servicio** de la ventana **Códs. grupo prod. serv. est.**  

## <a name="to-register-internal-or-public-comments"></a>Para registrar comentarios internos o públicos
Puede agregar comentarios que se imprimirán en los pedidos y ofertas de servicio para proporcionar información adicional. Puede agregar hasta 80 caracteres, incluso espacios. Si necesita escribir más texto, elija otra línea. Para registrar un comentario, elija una línea y, a continuación, elija la acción **Comentarios**.  

## <a name="to-delete-invoiced-service-orders"></a>Para eliminar pedidos de servicio facturados  
Los pedidos se suelen eliminar automáticamente después de haberse facturado en su totalidad. Cuando se registra una factura, se crea un movimiento correspondiente en la ventana **Facts. ventas (servicio) regis.** El documento registrado se puede ver en la página **Fact. ventas (servicio) regis.**  
  
Sin embargo, los pedidos de servicio no se eliminarán de forma automática si la cantidad total de dicho pedido no se ha registrado desde el pedido de servicio en sí, sino desde la ventana **Factura servicio**. En este caso, puede que tenga que eliminar los pedidos facturados que no se hayan eliminado. Para ello, ejecute el proceso **Eliminar ped. servicio facturados**.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Eliminar ped. servicio facturados** y, a continuación, seleccione el vínculo relacionado. Se abre la ventana de condiciones del trabajo por lotes **Eliminar pedidos de servicio facturados**.  
2. Para seleccionar los pedidos que se van a eliminar, puede definir filtros en los campos **Nº**, **Nº cliente** y **Factura Nº cliente**. .  
3. Elija el botón **Aceptar**.  


## <a name="see-also"></a>Consulte también  
[Registro de servicio](service-service-posting.md)  
[Cómo registrar un pedido de servicio](service-how-to-post-service-orders.md)  
[Configurar la gestión de servicios](service-setup-service.md)  
[Cómo trabajar en tareas de servicio](service-how-to-work-on-service-tasks.md)  
[Asignar recursos](service-how-to-allocate-resources.md)  

