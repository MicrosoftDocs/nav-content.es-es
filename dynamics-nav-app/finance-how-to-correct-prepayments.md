---
title: "Cómo corregir prepagos"
description: "Puede corregir un pedido después de haber registrado una factura de prepago para el mismo. Puede agregar nuevas líneas a un pedido después de emitir un prepago y, a continuación, registrar otra factura de prepago, pero no puede eliminar una línea de un pedido una vez que se haya facturado un prepago para la línea."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c39223940880514f9a59eae96e88182e19db2b5e
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-correct-prepayments"></a><span data-ttu-id="1630e-104">Cómo corregir prepagos</span><span class="sxs-lookup"><span data-stu-id="1630e-104">How to: Correct Prepayments</span></span>
<span data-ttu-id="1630e-105">Puede corregir un pedido después de haber registrado una factura de prepago para el mismo.</span><span class="sxs-lookup"><span data-stu-id="1630e-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span></span> <span data-ttu-id="1630e-106">Puede agregar nuevas líneas a un pedido después de emitir un prepago y, a continuación, registrar otra factura de prepago, pero no puede eliminar una línea de un pedido una vez que se haya facturado un prepago para la línea.</span><span class="sxs-lookup"><span data-stu-id="1630e-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span></span>  

## <a name="to-correct-a-prepayment"></a><span data-ttu-id="1630e-107">Para corregir un prepago</span><span class="sxs-lookup"><span data-stu-id="1630e-107">To correct a prepayment</span></span>
<span data-ttu-id="1630e-108">El procedimiento siguiente muestra cómo emitir una abono de prepago para cancelar todos los pagos adelantados facturados para un pedido de venta.</span><span class="sxs-lookup"><span data-stu-id="1630e-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span></span>  
1. <span data-ttu-id="1630e-109">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="1630e-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1630e-110">Abra el pedido de venta correspondiente.</span><span class="sxs-lookup"><span data-stu-id="1630e-110">Open the relevant sales order.</span></span>
3. <span data-ttu-id="1630e-111">Elija la acción **Prepago** y **Registrar abono prepago** o **Registrar e imprimir abono prepago**.</span><span class="sxs-lookup"><span data-stu-id="1630e-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span></span>  
4. <span data-ttu-id="1630e-112">En la ventana **Abono venta**, corrija los movimientos correspondientes, en función de cualquier abono de venta.</span><span class="sxs-lookup"><span data-stu-id="1630e-112">In the **Sales Credit Memo** window, proceed to correct the relevant entries, as for any sales credit memo.</span></span> <span data-ttu-id="1630e-113">Para obtener más información, vea [Procedimiento: Procesar devoluciones de ventas o cancelaciones](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="1630e-113">For more information, see [How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>     

    > [!NOTE]  
    > <span data-ttu-id="1630e-114">Para reducir la cantidad del campo **Importe de línea**, antes debe aumentar el porcentaje de prepago de la línea, para que el valor del campo **Importe línea prepago** no se reduzca por debajo del valor del campo **Importe prepago facturado**.</span><span class="sxs-lookup"><span data-stu-id="1630e-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span></span>

5. <span data-ttu-id="1630e-115">Para crear una factura prepago para las nuevas líneas en el abono de ventas, elija las acciones **Prepago** y **Registrar factura prepago** o **Registrar e imprimir factura prepago**.</span><span class="sxs-lookup"><span data-stu-id="1630e-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span></span>  
6. <span data-ttu-id="1630e-116">Para emitir una factura de prepago adicional, aumente la cantidad de prepago de una o varias líneas y registre la factura de prepago.</span><span class="sxs-lookup"><span data-stu-id="1630e-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span></span> <span data-ttu-id="1630e-117">Se creará una nueva factura con la diferencia entre las cantidades de prepago facturadas y las nuevas cantidades de prepago.</span><span class="sxs-lookup"><span data-stu-id="1630e-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1630e-118">Consulte también</span><span class="sxs-lookup"><span data-stu-id="1630e-118">See Also</span></span>  
[<span data-ttu-id="1630e-119">Facturación de prepagos</span><span class="sxs-lookup"><span data-stu-id="1630e-119">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="1630e-120">Tutorial: Configuración y facturación de prepagos de ventas</span><span class="sxs-lookup"><span data-stu-id="1630e-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="1630e-121">Finanzas</span><span class="sxs-lookup"><span data-stu-id="1630e-121">Finance</span></span>](finance.md)  
<span data-ttu-id="1630e-122">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1630e-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
