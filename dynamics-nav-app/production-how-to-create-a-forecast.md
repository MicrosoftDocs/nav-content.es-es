---
title: "Creación de una previsión de producción"
description: "Es posible crear previsiones de ventas y producción desde la ventana **Previsión de producción**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 106e75dbe6f1fca00ba09a19eeafb965fa83f4ea
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-a-production-forecast"></a>Creación de una previsión de producción
Es posible crear previsiones de ventas y producción desde la ventana **Previsión de producción**.  

La funcionalidad de previsión se utiliza para crear la demanda prevista; la demanda real se crea a partir de las ventas y los pedidos de producción. Durante la creación del Programa de producción principal (MPS), la previsión se liquida con las ventas y los pedidos de producción. La opción *Componente* de la previsión determina qué tipo de requisitos se deben tener en cuenta en el proceso de liquidación. Si la previsión es para un producto de venta, sólo se liquidan los pedidos de venta en la previsión. Si es para componentes, sólo se liquida la demanda que depende de los componentes de la orden de producción en la previsión.  

Mediante la previsión, la empresa puede crear escenarios hipotéticos y planificar y satisfacer la demanda con eficacia y rentabilidad. Una previsión exacta puede aumentar significativamente el grado de satisfacción de los clientes en relación con el cumplimiento de fechas y la entrega puntual.  

## <a name="sales-forecasts-and-production-forecasts"></a>Previsiones de ventas y previsiones de producción  
La funcionalidad de previsión del sistema se puede usar para crear previsiones de ventas o de producción, juntas o por separado. Por ejemplo, casi todas las empresas que fabrican contra pedido no disponen de existencias de productos terminados, porque cada producto se fabrica cuando se pide. La previsión de pedidos (previsión de ventas) es esencial para lograr unos plazos de producción de los productos terminados razonables (previsión de producción). Por ejemplo, si las piezas de los componentes tienen tiempos de entrega muy largos, y no están pedidas o en existencias, pueden retrasar la producción.  

-   La previsión de ventas es la mejor previsión del departamento del mismo nombre de lo que se va a vender en el futuro, y se determina por producto y por periodo. Con todo, la previsión de ventas no es siempre adecuada para la producción.  
-   La elaboración de previsiones es la proyección del planificador de producción de cuántos productos finales y productos semiterminados derivados se deben producir en cada periodo específico para cubrir las ventas previstas.  

En la mayoría de los casos, el responsable de la planificación de la producción modifica la previsión de ventas para ajustarla a las condiciones de producción, si bien debe satisfacer la previsión de ventas.  

Las previsiones se crean manualmente en la ventana **Previsión de producción**. En el sistema puede haber muchas previsiones, que se distinguen por el nombre y el tipo. Las previsiones se pueden copiar y editar como sea necesario. Tenga en cuenta que, en un momento dado, sólo se puede usar una previsión para realizar la planificación.  

La previsión está formada por una serie de registros, cada uno de los cuales debe tener un número de producto, una fecha de previsión y una cantidad prevista. La previsión de un producto abarca un periodo de tiempo, definido mediante la fecha de previsión y la fecha de previsión del siguiente registro de la previsión. Desde el punto de vista de la planificación, la cantidad prevista debe estar disponible al principio del periodo de demanda.  

Debe calificar una previsión como de *Producto venta*, *Componente* o *Ambos*. El tipo de previsión *Producto venta* se usa en la previsión de ventas. La previsión de producción se crea con el tipo *Componente*. El tipo de previsión *Ambos* sólo se usa para ofrecer al responsable de la planificación una visión general de las previsiones de ventas y de producción. Con esta opción, los movimientos de previsión no se pueden modificar. Mediante la calificación de estos tipos de previsión aquí, puede usar la misma hoja para introducir una previsión de ventas de la misma forma que se introduce una previsión de producción, y usar la misma hoja para ver las dos previsiones a la vez. Tenga en cuenta que el sistema trata los dos tipos de información (ventas y producción) de distinta forma al calcular la planificación, en función de la configuración del producto, la fabricación y la producción.  

## <a name="component-forecast"></a>Previsión de componentes  
La previsión de componentes es una previsión en relación con un producto principal. Puede resultar útil, por ejemplo, si el responsable de la planificación puede estimar la demanda del componente.  

Dado que la previsión de componentes está diseñada para definir las opciones de un producto principal, debe ser igual a o menor que la cantidad prevista del producto de venta. Si la previsión de componentes es mayor que la previsión del producto de venta, el programa considera la diferencia entre los dos tipos de previsión como demanda independiente.  

## <a name="forecasting-periods"></a>Periodos de previsión  
 El periodo de previsión es válido desde la fecha de inicio hasta la fecha de inicio de la siguiente previsión. La ventana de intervalo de tiempo proporciona muchas opciones para insertar la demanda en una fecha concreta del periodo. Por ello, es aconsejable no cambiar el periodo de previsión salvo que se desee llevar todos los movimientos a la fecha de inicio de este periodo.  

## <a name="forecast-by-locations"></a>Previsión por ubicación  
Se puede establecer en la configuración de la fabricación. Con todo, debe tener en cuenta que si las previsiones en función de las ubicaciones se observan por separado, la previsión global podría no ser representativa.

## <a name="to-create-a-production-forecast"></a>Creación de una previsión de producción

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Previsión de producción** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione una previsión en el campo **Nombre previsión producción** de la ficha desplegable **General**. Puede haber varias previsiones, que se distinguen por el nombre y el tipo de previsión.  
3.  Seleccione el almacén del campo **Filtro almacén** al que se va a aplicar esta previsión.  
4.  En el campo **Tipo previsión**, seleccione **Producto venta**, **Componente** o **Ambos**. Si selecciona **Producto venta** o **Componente**, puede editar la cantidad según el periodo. Si selecciona **Ambos**, no podrá modificar la cantidad, pero podrá elegir el botón de flecha desplegable y ver los movimientos de previsión de producción.  
5.  Especifique un **Filtro fecha** si desea limitar la cantidad de datos que se muestran.  
6.  Introduzca las cantidades previstas de **Producto venta** o **Componente** para los distintos periodos en la ficha desplegable **Matriz prev. producción**.  
7.  Para modificar el periodo que se muestra en cada columna, ajuste el intervalo de tiempo en el campo **Ver por** de la ficha desplegable **Opciones matriz**. Se pueden seleccionar los siguientes intervalos: **Día**, **Semana**, **Mes**, **Trimestre**, **Año** o el **Periodo contable**, configurado en la Gestión financiera.  

    > [!NOTE]  
    >  Debería analizar qué intervalo de tiempo desea utilizar para futuras previsiones para que sea el mismo en todas las ocasiones. Si especifica una cantidad de previsión, es válida el primer día del intervalo de tiempo seleccionado. Por ejemplo, si selecciona un mes, debe especificar la cantidad prevista en el primer día del mes. Si selecciona un trimestre, debe especificar la cantidad del primer día del primer mes del trimestre.  

8.  Seleccione cómo se mostrarán las cantidades de previsión del intervalo de tiempo en el campo **Ver como**. Si se selecciona **Saldo periodo**, se mostrará el balance del saldo del periodo. Si se selecciona **Saldo a la fecha**, la ventana mostrará el saldo del último día del intervalo de tiempo.  

> [!NOTE]  
>  También se puede editar una previsión existente. Haga clic en la ventana **Matriz de prevision de producción.**, seleccione la acción **Copiar previsión de producción** y rellene la ventana **Previsión de producción** con una previsión existente. Es posible realizar modificaciones a las cantidades según sea pertinente.  

## <a name="see-also"></a>Consulte también  
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Detalles de diseño: planificación de aprovisionamiento](design-details-supply-planning.md)   
[Procedimientos recomendados de configuración: planificación de suministros](setup-best-practices-supply-planning.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

