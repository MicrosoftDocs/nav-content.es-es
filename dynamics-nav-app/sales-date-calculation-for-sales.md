---
title: "Cálculo de fecha de ventas"
description: "El programa calcula automáticamente la fecha en la que se debe solicitar un producto para tenerlo en el inventario en una fecha determinada. Esta es la fecha en la que puede contar con que los productos solicitados en una fecha determinada estén disponibles para picking."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 72e8f2a2f1d2d6427c716205da7ecee58b85bcc6
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-sales"></a><span data-ttu-id="34571-104">Cálculo de fecha de ventas</span><span class="sxs-lookup"><span data-stu-id="34571-104">Date Calculation for Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="34571-105"> calcula automáticamente la fecha más próxima posible en la que se puede enviar un producto incluido en una línea de pedido de venta.</span><span class="sxs-lookup"><span data-stu-id="34571-105"> automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span></span>

<span data-ttu-id="34571-106">Si el cliente solicita una fecha de entrega concreta, se calcula la fecha en que los productos deberán estar disponibles para el picking y poder realizar su entrega en dicha fecha.</span><span class="sxs-lookup"><span data-stu-id="34571-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span></span>

<span data-ttu-id="34571-107">Si el cliente no solicita una fecha de entrega concreta, se calcula la fecha en que los productos se podrán entregar, a partir de la fecha en que estén disponibles para el picking.</span><span class="sxs-lookup"><span data-stu-id="34571-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span></span>

## <a name="calculating-a-requested-delivery-date"></a><span data-ttu-id="34571-108">Realizar cálculos de una Fecha de entrega requerida</span><span class="sxs-lookup"><span data-stu-id="34571-108">Calculating a Requested Delivery Date</span></span>
<span data-ttu-id="34571-109">Si escribe una fecha de entrega requerida en la línea de pedido de venta, se utilizará dicha fecha como punto inicial para los cálculos siguientes.</span><span class="sxs-lookup"><span data-stu-id="34571-109">If you specify a requested delivery date on the sales order line, then that date is used as the starting point for the following calculations.</span></span>

- <span data-ttu-id="34571-110">Fecha entrega requerida - Hora envío = Fecha envío planeada</span><span class="sxs-lookup"><span data-stu-id="34571-110">requested delivery date - shipping time = planned shipment date</span></span>
- <span data-ttu-id="34571-111">Fecha envío planeada - Tiempo manip. alm. salida = Fecha envío</span><span class="sxs-lookup"><span data-stu-id="34571-111">planned shipment date - outbound whse. handling time = shipment date</span></span>

<span data-ttu-id="34571-112">Si los productos están disponibles para el picking en la fecha de envío, el proceso de venta puede continuar.</span><span class="sxs-lookup"><span data-stu-id="34571-112">If the items are available to pick on the shipment date, then the sales process can continue.</span></span>

<span data-ttu-id="34571-113">Si no lo están, se mostrará la advertencia de falta de stock.</span><span class="sxs-lookup"><span data-stu-id="34571-113">If the items are not available to be picked on the shipment date, then a stock-out warning is displayed.</span></span>

## <a name="calculating-the-earliest-possible-delivery-date"></a><span data-ttu-id="34571-114">Cálculo de fecha de entrega más próxima posible</span><span class="sxs-lookup"><span data-stu-id="34571-114">Calculating the Earliest Possible Delivery Date</span></span>
<span data-ttu-id="34571-115">Si no especifica una fecha de entrega requerida en la línea de pedido de venta, o si la fecha de entrega requerida no se puede cumplir, se calculará la fecha más próxima en la que estarán disponibles los productos.</span><span class="sxs-lookup"><span data-stu-id="34571-115">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span></span> <span data-ttu-id="34571-116">A continuación se insertará dicha fecha en la línea del campo Fecha envío y utiliza las siguientes formulas para calcular la fecha prevista para el envío de los productos y la fecha de su entrega al cliente:</span><span class="sxs-lookup"><span data-stu-id="34571-116">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span></span>

- <span data-ttu-id="34571-117">Fecha envío + Tiempo manip. alm. salida = Fecha envío planeada</span><span class="sxs-lookup"><span data-stu-id="34571-117">shipment date + outbound whse. handling time = planned shipment date</span></span>
- <span data-ttu-id="34571-118">Fecha envío planeada + Hora envío = Fecha entrega planeada</span><span class="sxs-lookup"><span data-stu-id="34571-118">planned shipment date + shipping time = planned delivery date</span></span>


## <a name="see-also"></a><span data-ttu-id="34571-119">Consulte también</span><span class="sxs-lookup"><span data-stu-id="34571-119">See Also</span></span>  
 <span data-ttu-id="34571-120">[Cálculo de la fecha de compras](purchasing-date-calculation-for-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="34571-120">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span></span>  
 [<span data-ttu-id="34571-121">Procedimiento: cálculo de las fechas de compromiso de entrega de pedido</span><span class="sxs-lookup"><span data-stu-id="34571-121">How to: Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="34571-122">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="34571-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
