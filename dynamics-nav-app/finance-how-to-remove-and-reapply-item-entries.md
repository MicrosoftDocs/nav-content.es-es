---
title: "Cómo eliminar y liquidar de nuevo los movimientos de producto"
description: "Puede ver y modificar manualmente determinados movimientos de liquidación del producto que se crean automáticamente durante las transacciones del inventario."
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
ms.openlocfilehash: 400a30ab196d2015bd9caae3fcb38dfdceea53ca
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-remove-and-reapply-item-ledger-entries"></a>Cómo eliminar y liquidar de nuevo los movimientos contables de producto
En la ventana **Hoja liquidación**, puede ver y modificar manualmente determinados movimientos de liquidación del producto que se crean automáticamente durante las transacciones del inventario.  

Cuando registra una transacción en la que entran o salen productos del inventario, se crea una liquidación de producto entre cada aumento y disminución de inventario. Dichas liquidaciones determinan el flujo de costes desde los bienes que se reciben en el inventario al coste de los bienes que salen del inventario. Debido a la forma en la que se calcula el coste unitario, una liquidación de producto que sea incorrecta podría resultar en un coste medio sesgado y en un coste unitario también sesgado. Para obtener más información, consulte Detalles de diseño: Liquidación de productos.

Es posible que en los siguientes ejemplos, sea necesario deshacer una liquidación o volver a liquidar movimientos de productos:

- Ha olvidado realizar una liquidación fija.
- Ha realizado una liquidación fija incorrecta.
- Debe devolver un producto al que ya se ha aplicado una venta.

Si es posible, utilice un documento para volver a liquidar un movimiento de producto. Por ejemplo, si necesita realizar una devolución de compra de un producto al que ya se ha aplicado una venta, puede realizar una repetición de la liquidación creando y registrando el documento de devolución de compra utilizando la liquidación correcta en el campo **Liq. por nº orden producto** situado en la línea de devolución de compra. Puede utilizar la función **Revertir líneas documentos registrados** o la función **Copiar líneas** en el documento de devolución de compra para facilitar este proceso. Cuando registra el documento, el movimiento de producto se vuelve a liquidar automáticamente. Para obtener más información, vea [Procedimiento: Procesar devoluciones de compra o cancelaciones](purchasing-how-process-purchase-returns-cancellations.md).

Si no puede usar un documento para volver a liquidar, por ejemplo cuando tiene que corregir una liquidación fija, utilice la ventana **Hoja liquidación** para realizar la corrección.

> [!Warning]  
> A continuación se muestran algunos aspectos importantes que es necesario tener en cuenta a la hora de trabajar con la hoja de liquidación:
    - No debe dejar movimientos de liquidación sin liquidar durante largos periodos porque otros usuarios no pueden procesar los productos hasta que vuelve a liquidar los movimientos de liquidación o cierra la ventana **Hoja liquidación**. Los usuarios que intentan realizar acciones relacionadas con un movimiento de liquidación manualmente no liquidado recibirán el mensaje de error siguiente: “No se puede realizar esta acción porque los movimientos para el producto XXX no están liquidados en la Hoja de liquidación del usuario XXX”.
    - Es recomendable llevar a cabo el proceso de repetición de la liquidación sólo fuera del horario laboral para evitar conflictos con otros usuarios que estén registrando transacciones relacionadas con los mismos productos.
    - Cuando cierre la hoja de liquidación, [!INCLUDE[d365fin](includes/d365fin_md.md)] llevará a cabo una comprobación para asegurarse de que se han liquidado todos los productos. Por ejemplo, si elimina una liquidación de cantidad pero no crea una nueva liquidación y, a continuación, cierra la hoja de liquidación, se creará una nueva liquidación. Esto permite garantizar que los costes se mantengan intactos. No obstante, si elimina una liquidación fija, no se creará automáticamente una liquidación fija nueva cuando cierre la hoja de liquidación. Deberá hacerlo manualmente creando una nueva liquidación desde la hoja de liquidación.
    - Es posible eliminar liquidaciones de más de un movimiento a la vez desde la hoja de liquidación. Sin embargo, dado que la liquidación de movimientos afecta al conjunto de movimientos disponibles para ser liquidados, no es posible crear una liquidación para más de un movimiento a la vez.
    - La hoja de liquidación no puede realizar una liquidación si se da el caso siguiente: si no hay suficiente cantidad que liquidar en el stock, la hoja de liquidación no puede llevar a cabo el proceso si intente liquidar un movimiento de salida de existencias que no incluya información de seguimiento del producto con un movimiento de salida de existencias que sí incluya información de seguimiento.

## <a name="to-remove-an-item-application-by-using-the-application-worksheet"></a>Para eliminar una liquidación de producto con la Hoja de liquidación  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja liquidación** y, a continuación, seleccione el vínculo relacionado.  
2.  La ventana **Hoja liquidación** se abre y muestra los movimientos de producto existentes para todos los productos.  
3.  Especifique los filtros en la ficha desplegable **General** para facilitar el movimiento del producto para el cual desea cambiar la liquidación.  
4.  Seleccione el movimiento de producto relevante y, a continuación, seleccione la acción **Movs. liquidados**. Se abre la ventana **Ver, Movs. conciliados - Movs. conciliados** para mostrar los movimientos de producto que se aplican actualmente al movimiento seleccionado.  
5.  Seleccione aquel para el cual desea eliminar la liquidación.  
6.  Seleccione la acción **Eliminar liquidación**. De esta forma, se elimina el movimiento de liquidación del producto que vincula los dos movimientos y lo traslada a la ventana **Ver movs. conciliados - Movs. sin conciliar**.  
7.  Cierre la ventana **Ver, Movs. conciliados - Movs. conciliados**.  

 El campo **Cantidad pendiente** de los dos movimientos de producto aumenta según la cantidad que se ha desliquidado. El movimiento de producto eliminado está ya disponible para la nueva liquidación en la ventana **Ver movs. conciliados - Movs. sin conciliar**.  

> [!IMPORTANT]  
>  No debe dejar movimientos de liquidación sin liquidar durante periodos más largos porque otros usuarios no pueden procesar los productos afectados hasta que vuelva a liquidar los movimientos o cierre la ventana **Hoja liquidación**. Se muestra el mensaje de error siguiente si intenta realizar acciones relacionadas con un movimiento de liquidación no aplicado manualmente:  
>   
>  **No puede realizar esta acción porque los movimientos del producto <item> no están liquidados en la Hoja de liquidación del usuario <user>.**  

## <a name="to-reapply-an-item-application-by-using-the-application-worksheet"></a>Para volver a liquidar un producto con la Hoja liquidación  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja liquidación** y, a continuación, seleccione el vínculo relacionado.  
2.  La ventana **Hoja liquidación** se abre y muestra los movimientos de producto existentes para todos los productos.  
3.  Para volver a liquidar los movimientos eliminados desde que abriera la hoja de trabajo, seleccione el movimiento del producto que le gustaría volver a liquidar. En la pestaña **Acciones**, en el grupo **Funciones**, seleccione **Volver a liquidar**.  

    > [!NOTE]  
    >  Esta nueva liquidación en el saldo original también se produce automáticamente cuando cierra la ventana **Hoja liquidación**.  
4.  Para aplicar un movimiento de producto abierto disponible a otro movimiento, seleccione el movimiento de producto que desea aplicar. Seleccione la acción **Movs. no liquidados**. Se abre la ventana **Ver movs. conciliados - Movs. sin conciliar**.  
5.  Seleccione uno o más movimientos que desee liquidar en el movimiento seleccionado en la ventana **Hoja liquidación** y, a continuación, elija el botón **Aceptar**.  

     Se crea un movimiento de liquidación del producto entre ambos movimientos. Los campos **Cantidad pendiente** de ambos movimientos se verán reducidos por la cantidad liquidada.  

    > [!NOTE]  
    >  Si ha elegido llevar a cabo una liquidación que creará un bucle infinito en el proceso de ajuste del coste, la liquidación que ha propuesto no se realiza. Esto puede ocurrir cuando los movimientos originales han creado stock negativo. La liquidación no se realiza. Por tanto, debe seleccionar un movimiento diferente para la liquidación.  
6.  Si en la configuración de existencias, el campo **Ajuste automático coste** en **Configuración inventario** se ha establecido en **Siempre**, se ejecuta automáticamente el trabajo por lotes de ajuste del coste una vez que se haya repetido la liquidación De lo contrario, ejecute el trabajo por lotes **Valorar stock - movs. producto** para asegurarse de que todos los costes estén actualizados.  

## <a name="see-also"></a>Consulte también  
[Cómo cerrar los movimientos de producto abiertos que se crean por una liquidación fija en el diario de productos](finance-how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal.md)  
 [Procesamiento de devoluciones de compra o cancelaciones](purchasing-how-process-purchase-returns-cancellations.md)  
 [Gestión de costes de inventario](finance-manage-inventory-costs.md)   
 [Detalles de diseño: Liquidación de productos](design-details-item-application.md)  
 [Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

