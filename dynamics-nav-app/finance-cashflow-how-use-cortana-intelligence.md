---
title: 'Procedimiento: crear previsiones de flujo de efectivo predictivas'
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 1fdb53b0f58ada22475fe1c1510146c156a60410
ms.contentlocale: es-es
ms.lasthandoff: 10/23/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Procedimiento: crear previsiones de flujo de efectivo predictivas
Las previsiones de flujo de efectivo ayudan a garantizar que su empresa dispone de suficiente efectivo disponible para cumplir las obligaciones financieras y son útiles para identificar ajustes. Por ejemplo, si tiene un exceso de efectivo podría pagar algunas deudas, y apreciará una advertencia temprana si vienen tiempos difíciles.

Cortana Intelligence usa el servicio Azure Machine Learning para realizar previsiones confiables y predictivas. Por ejemplo, las previsiones de Cortana Intelligence pueden ayudarle a predecir y evitar los déficits de efectivo. El servicio combina la información histórica con los registros actuales para pagos y cobros, incluidos los registros cuya fecha de vencimiento sea en el futuro. Se incluyen:
* Pedidos de compra
* Pedidos venta
* Facturas de ventas y de compras registradas
* Abonos

## <a name="before-you-start"></a>Antes de comenzar  
Debe hacer algunas cosas para usar Cortana Intelligence para las previsiones del flujo de efectivo:
* Si todavía no usa las previsiones del flujo de efectivo, deberá configurar:
    * Una o más configuraciones en **Configuración flujos efectivo**.
    * Cuentas para pagos, cobros, pedidos de venta y pedidos de compra. Cortana Intelligence usa los registros en estas cuentas.
    * Una o más previsiones de flujo de efectivo en **Previsión de flujo de efectivo**. Asegúrese de incluir pedidos de compra, los pedidos de venta, cobros y pagos como orígenes.  
    Para obtener más información, busque _previsiones de flujo de efectivo_ en el sistema de Ayuda.
* Debe conocer la URL de API y la clave de API del servicio web de previsión que usará.  
    Puede utilizar Azure Machine Learning u otro servicio, si lo tiene. Opcionalmente, hay disponible un modelo público denominado _modelo de previsión para Microsoft Dynamics NAV_ en la galería de Cortana Intelligence. Para usar el modelo, siga estos pasos:

    1. En el explorador, vaya a la [Galería de Cortana Intelligence](https://go.microsoft.com/fwlink/?linkid=828352).
    2. Busque _Modelo de previsión para Microsoft Dynamics NAV_ y, a continuación, abra el modelo en Azure Machine Learning Studio.
    3. Use su cuenta de Microsoft para iniciar sesión en un espacio de trabajo y, a continuación, copie el modelo.
    4. Ejecute el modelo y como publíquelo como un servicio web.
    5. Anote la URL de API y la clave de API. Usará estas credenciales al configurar Cortana Intelligence en [!INCLUDE[navnow](includes/navnow_md.md)].  

* Considere la frecuencia con que se calculará la previsión. El servicio Azure Machine Learning tiene limitaciones en cuanto al uso. Por ejemplo, si tiene muchos productos, podría ser mejor calcular con menos frecuencia.
* Asígnese al área de trabajo Contable.

## <a name="set-up-cortana-intelligence"></a>Configurar Cortana Intelligence
Puede usar una guía de configuración asistida para configurar las previsiones del flujo de efectivo. Esta guía le ayuda a especificar aspectos como la frecuencia con que se actualizará la previsión, las cuentas en las que se basará, la información acerca de cuándo se pagan impuestos y si se usa Cortana Intelligence.  

Si ya usa previsiones de flujo de efectivo y solo desea activar Cortana Intelligence., también puede usar un proceso manual. Cuando inicie sesión, se mostrará una notificación en una barra azul en la parte superior del espacio de trabajo. Para configurar Cortana Intelligence inmediatamente, elija **Sí**. El mensaje solo se muestra una vez. Si lo cierra, use el proceso manual para configurar Cortana Intelligence.  

**Sugerencia:** considere la duración de los periodos que el servicio usará en los cálculos. Cuantos más datos proporcione, más precisas serán las predicciones. Asimismo, controle las variaciones grandes en los periodos. También afectarán a las predicciones. Si Cortana Intelligence no encuentra suficientes datos, o los datos varían mucho, el servicio no creará ninguna predicción.

Para usar la guía de configuración asistida:
1. En el área de trabajo Contable, en el gráfico **Previsión de flujo de efectivo**, elija la acción **Abrir Configuración asistida**.
2. Rellene los campos según sea necesario en cada paso de la guía.

Para usar un proceso manual:
1. Busque **Configuración flujos de efectivo** y, a continuación, elija el vínculo relacionado.
2. Expanda la ficha desplegable **Cortana Intelligence** y, a continuación, rellene los campos según sea necesario.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Activar Cortana Intelligence para las previsiones de flujo de efectivo
1. Busque **Previsiones de flujo de efectivo** y, a continuación, elija el vínculo relacionado.
2. Elija la acción **Hoja flujos efectivo**.
3. En la página **Hoja flujos efectivo**, elija la acción **Proponer líneas de hoja de trabajo**.  
4. En **Tipos de orígenes para incluir**, elija la casilla **Previsión de Cortana Intelligence**.

## <a name="investigate-a-cash-flow-forecast"></a>Investigar una previsión del flujo de efectivo
Para examinar los datos subyacentes a la previsión, incluida la varianza, elija la columna **Cortana Intelligence**. La primera fila de la tabla muestra la varianza. Las demás filas están organizadas por el documento de origen.  

Por ejemplo, puede ver cómo la previsión:    
* Controla las ventas y las compras confirmadas
* Resta los pagos y suma los cobros
* Omite los pedidos de venta y de compra duplicados

## <a name="see-also"></a>Consulte también  
[Trabajar con Dynamics NAV](ui-work-product.md)

