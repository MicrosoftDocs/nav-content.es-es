---
title: "Establecer límites para fechas de vencimiento"
description: "Puede modificar los términos de pago para que tengan límites para la cantidad máxima de días que puede transcurrir entre una entrega y el pago correspondiente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dfac0333a31e65977d38fa75077bf3d7708208a8
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-limits-for-due-dates"></a>Establecer límites para fechas de vencimiento
Puede modificar los términos de pago para que tengan límites para la cantidad máxima de días que puede transcurrir entre una entrega y el pago correspondiente.  

 Los límites legales del espacio entre su entrega y pago determinan cómo se calculan las fechas de vencimiento. Por ejemplo, si crea un término de pago que se utilizará para ventas al sector público, el campo **Nº máx. días hasta fecha vencimiento** para ese plazo de pago debe establecerse en 30 días.  

### <a name="to-set-limits-for-due-dates-on-payment-terms"></a>Para definir los límites para las fechas de vencimiento en términos de pago  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Condiciones de pago** y, a continuación, seleccione el vínculo relacionado.  

2.  Seleccione el término de pago que desea modificar y, a continuación, en el campo **Nº máx. días hasta fecha vencimiento**, especifique el número de días naturales permitidos entre su entrega y el pago.  

 A continuación, debe asegurarse de especificar los términos de pago adecuados para sus clientes y proveedores públicos y privados. Cuando crea un documento para ese cliente o proveedor, la fecha de vencimiento del pago se calcula a partir del día en que el cliente recibió los artículos o servicios. A continuación, debe actualizar el campo **Fecha del documento** con la fecha del recibo. Por ejemplo, si actualiza una factura de ventas cuando se le informa de la entrega, la fecha de vencimiento se calcula en función de la nueva fecha del documento que especificó. La fecha de vencimiento calculada no puede superar el límite que especificó para el plazo de pago.  

> [!IMPORTANT]  
>  No puede registrar un documento que crea una remesa donde uno o varios plazos tienen una fecha de vencimiento posterior al límite que se especifica en el campo **Nº máx. días hasta fecha vencimiento**.  

## <a name="see-also"></a>Consulte también  
 [Cálculo de fechas de vencimiento](calculating-due-dates.md)   
 [Configuración de términos de pago](../../how-to-set-up-payment-terms.md)

