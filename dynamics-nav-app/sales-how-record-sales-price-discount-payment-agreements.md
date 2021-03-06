---
title: Configurar precios y descuentos de venta especiales para clientes
description: "Describe cómo definir los acuerdos de precios y descuentos alternativos que desea aplicar a los documentos de venta al vender a distintos clientes."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: special price, alternate price, pricing
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 980e6e117887e0a0dab68aedfa99f99c27b876c9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-record-special-sales-prices-and-discounts"></a>Registrar precios y descuentos de venta especiales
Es necesario definir los acuerdos de precios y descuentos que se aplican al vender a distintos clientes de modo que se apliquen las reglas y valores acordados a los documentos de venta que cree para los clientes.

Cuando haya registrado precios especiales y los descuentos de línea para ventas y compras, [!INCLUDE[d365fin](includes/d365fin_md.md)] garantiza que el beneficio en operaciones comerciales de producto siempre son óptimos calculando automáticamente el mejor precio en los documentos de ventas y compras, y en líneas del diario de proyectos y recursos. Para obtener más información, consulte la sección "Cálculo del mejor precio".

Respecto a los precios, puede tener una precio especial de venta insertado en las líneas de venta si existe una cierta combinación de cliente, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin.

Respecto a los descuentos, puede configurar y usar dos tipos de descuentos de ventas:

| Tipo de descuento | Descripción |
| --- | --- |
| **Descuento línea venta** |Un importe de descuento que está insertado en las líneas de venta si existe una cierta combinación de cliente, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin. Funciona igual que para los precios de venta. |
| **Descuento en factura** |Un porcentaje de descuento que se resta del total del documento si el importe de todas las líneas de un documento de venta supera cierto límite. |

Dado que los descuentos de línea de venta y los precios de venta se basan en una combinación de producto y cliente, también puede basar esta configuración en la ficha del producto al que se aplican las reglas y valores.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Para configurar un precio de venta para un cliente
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de cliente correspondiente y, a continuación, elija la acción **Precios**.

    El campo **Tipo venta** se rellena con **Cliente**y el campo **Código ventas** se rellena con el número de cliente.
3. Rellene los campos de la línea como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Rellene una línea para cada combinación que aplicará un precio de venta especial al cliente.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Para configurar un descuento de línea de venta para un cliente
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de cliente correspondiente y, a continuación, elija la acción **Dto. línea**.

    El campo **Tipo venta** se rellena con **Cliente**y el campo **Código ventas** se rellena con el número de cliente.
3. Rellene los campos de la línea como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Rellene una línea para cada combinación que aplicará un descuento de línea de venta al cliente.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Para configurar un descuento en factura para un cliente
Una vez que haya determinado los clientes que pueden obtener descuentos en factura, introduzca el código de descuento en factura en las fichas de cliente y especifique los términos de cada código.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un cliente que pueda obtener descuentos en factura.
3. En el campo **Código descuento factura**, seleccione un código para los términos relevantes de la factura con descuentos que usará para calcular los descuentos en facturas para el cliente.

    > [!NOTE]  
>   Los códigos de descuento en factura se representan por las fichas existentes del cliente. Lo que permite asignar rápidamente las condiciones de descuento en factura a clientes realizando el picking del nombre de otros clientes con los mismos términos.

    Configure de nuevo los términos de descuento en factura para ventas.
4. En la ventana **Ficha de cliente**, seleccione la acción **Descuento factura**. Aparecerá la ventana **Dtos. factura cliente**.
5. En el campo **Código divisa**, introduzca el código de una divisa que se aplique a los términos de descuento en factura en la línea. Deje el campo en blanco para establecer condiciones de descuento de factura en USD.
6. En el campo **Importe mínimo**, escriba el importe mínimo que deba tener una factura para optar al descuento.
7. En el campo **% descuento**, introduzca el descuento en la factura como un porcentaje del importe de la factura.
8. Repita los pasos del 5 al 7 para cada divisa que el cliente reciba un descuento diferente de factura.

El descuento en factura ahora está configurado y asignado al cliente en cuestión. Al seleccionar el código del cliente en el campo **Cód. dto. factura** en otras fichas de cliente, se asigna el mismo descuento en factura a estos clientes.

## <a name="to-work-with-sales-invoice-discounts-and-service-charges"></a>Trabajar con descuentos y cargos por servicios de la factura de venta
Al utilizar descuentos en factura, el importe de la factura determina el descuento aplicado.  

En la ventana **Dtos. factura clientes**, también puede añadir un cargo por servicio a las facturas que superen un determinado importe.  

Para poder aplicar descuentos en factura a las ventas, primero debe especificar determinados datos en el sistema. Deberá determinar las siguientes cuestiones:  

- a qué clientes se le concederá este tipo de descuento.  
- qué porcentajes de descuento se va a aplicar.  

Si factura descuentos para que se calculen automáticamente, puede especificarlo en la ventana **Configuración ventas y cobros**.  

Decida si va a conceder o no descuentos en factura a cada cliente que cumpla el requisito (es decir, que el importe de su factura supere una determinada cantidad). Defina los términos de los descuentos en factura en divisa local para los clientes nacionales y en otras divisas para los clientes de otros países.  

Se relacionan los porcentajes de descuento a los importes de factura específicos en las ventanas **Dtos. factura cliente**. Puede introducir un número ilimitado de porcentajes en cada ventana. Cada cliente puede tener su propia ventana o se pueden vincular varios clientes a la misma ventana.  

Además de (o en lugar de) un porcentaje de descuento, puede vincular un importe de cargo por servicios a un importe facturado específico.  

> [!TIP]  
>  Antes de introducir esta información en el sistema, se recomienda preparar un esquema de la estructura de descuentos que desea utilizar. De este modo, podrá ver fácilmente los clientes que se pueden vincular a la misma ventana de descuentos en factura. Cuantas menos ventanas tenga que configurar, más rápido introducirá la información básica.  

## <a name="best-price-calculation"></a>Cálculo del mejor precio
Cuando haya registrado precios especiales y los descuentos de línea para ventas y compras, [!INCLUDE[d365fin](includes/d365fin_md.md)] garantiza que el beneficio en operaciones comerciales de producto siempre son óptimos calculando automáticamente el mejor precio en los documentos de ventas y compras, y en líneas del diario de proyectos y recursos.

El mejor precio es el precio más bajo permisible con el mayor descuento de línea permisible en una fecha indicada. [!INCLUDE[d365fin](includes/d365fin_md.md)] lo calcula automáticamente al insertar el precio por unidad y el porcentaje de descuento de línea de los productos en las nuevas líneas de documento y diario.

> [!NOTE]  
>   A continuación se describe cómo se calcula el mejor precio para las ventas. El cálculo es igual para las compras.

1. [!INCLUDE[d365fin](includes/d365fin_md.md)] comprueba la combinación de la factura a cliente y el producto, y calcula el precio por unidad y el porcentaje de descuento de línea aplicables utilizando los siguientes criterios:

    - ¿El cliente tiene un acuerdo de precios o descuentos, o el cliente pertenece a un grupo que lo tiene?
    - ¿Está incluido el producto o el grupo de descuento del producto de la línea en alguno de estos acuerdos de precios o descuentos?
    - ¿La fecha de pedido (o la fecha de registro de la factura y abono) está comprendida entre la fecha inicial y la fecha final del acuerdo de precios o descuentos?
    - ¿Se ha especificado un código de unidad de medida? Si es así, [!INCLUDE[d365fin](includes/d365fin_md.md)] comprueba los precios o descuentos con el mismo código de unidad de medida y los precios o descuentos sin un código de unidad de medida.

2. [!INCLUDE[d365fin](includes/d365fin_md.md)] comprueba si se aplican acuerdos de precios o de descuentos a la información de la línea de documento o de diario y, a continuación, inserta el precio unitario y porcentaje de descuento de línea, utilizando el siguiente criterio:

    - ¿Hay un requisito de cantidad mínima en el acuerdo de precios o descuentos que se debe cumplir?
    - ¿Hay un requisito de divisa en el acuerdo de precios o descuentos que se debe cumplir? Si es así, se insertan el precio más bajo y el descuento de línea más alto para esa divisa, incluso si la divisa local proporciona un precio mejor. Si no existen acuerdos de precios o descuentos para el código de divisa especificado, [!INCLUDE[d365fin](includes/d365fin_md.md)] inserte el menor precio y el mayor descuento de línea en la su divisa local.

Si no se puede calcular ningún precio especial para el producto de la línea, se inserta el último coste directo o el precio unitario de la ficha de producto.

## <a name="to-copy-sales-prices"></a>Para copiar precios de venta  
Si desea copiar precios de venta, por ejemplo, los precios de venta de un cliente determinado a un grupo de precio de cliente, debe ejecutar el proceso **Sugerir precio venta en hoja**. Trabajo por lotes . Este proceso se encuentra en la ventana **Hoja precios venta**.    

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja de precios de venta** y, a continuación, seleccione el vínculo relacionado.  
2.  Elija **Sugerir precio venta en hoja**. .  
3.  En la ficha desplegable **Precios venta**, rellene los campos **Tipo venta** y **Código ventas** con los precios de venta originales que desea copiar.  
4.  En la parte superior de la ventana de solicitud, rellene el **Tipo venta** y **Código ventas** con el tipo y el nombre al que desea copiar los precios de venta.  
5.  Si desea que el trabajo por lotes cree precios nuevos, seleccione el campo **Crear precios nuevos**.  
6.  Elija el botón **Aceptar** para rellenar las líneas de la ventana **Hoja precios venta** con los nuevos precios propuestos, indicando que son válidos para el **Tipo venta** seleccionado.  

> [!NOTE]  
>  El proceso sólo crea propuestas; no implementa los cambios propuestos. Si está satisfecho con las propuestas y desea implantarlas, es decir, insertarlas en la tabla **Precios de venta**, puede utilizar el trabajo por lotes **Realizar cambio precio**, que se encuentra en la pestaña **Acciones**, en el grupo **Funciones**, en la ventana **Hoja precios venta**.

## <a name="see-also"></a>Consulte también
[Configuración de ventas](sales-setup-sales.md)  
[Ccial](sales-manage-sales.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

