---
title: "Combinación de albaranes"
description: "Si desea facturar varios albaranes de compra a la vez, puede utilizar la función Combinar albaranes."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 10749dc8d8d692d94c5405fbb0a4a965d482f013
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a><span data-ttu-id="b7246-103">Procedimiento: agrupar albaranes en una factura única</span><span class="sxs-lookup"><span data-stu-id="b7246-103">How to: Combine Receipts on a Single Invoice</span></span>
<span data-ttu-id="b7246-104">Si desea facturar varios albaranes de compra a la vez, puede utilizar la función **Combinar albaranes**.</span><span class="sxs-lookup"><span data-stu-id="b7246-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span></span>  

<span data-ttu-id="b7246-105">Para poder crear un albarán de compra combinado, es necesario haber registrado primero más de un albarán del mismo proveedor y en la misma divisa.</span><span class="sxs-lookup"><span data-stu-id="b7246-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span></span> <span data-ttu-id="b7246-106">En otras palabras, debe haber rellenado dos o más pedidos de compra, así como haberlos registrado como recibidos, pero no facturado.</span><span class="sxs-lookup"><span data-stu-id="b7246-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span></span>  

<span data-ttu-id="b7246-107">Cuando se combinan varios albaranes de compra en una factura y se registran, se crea una factura de compra registrada para las líneas facturadas.</span><span class="sxs-lookup"><span data-stu-id="b7246-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span></span> <span data-ttu-id="b7246-108">El campo **Cantidad facturada** del pedido de compra de origen, o del pedido abierto de compra, se actualiza en función de la cantidad facturada.</span><span class="sxs-lookup"><span data-stu-id="b7246-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span></span> <span data-ttu-id="b7246-109">Sin embargo, este documento de compra original no se elimina, aunque se haya recibido y facturado por completo, por lo que debe eliminar el documento de compra.</span><span class="sxs-lookup"><span data-stu-id="b7246-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span></span>  

## <a name="to-combine-receipts"></a><span data-ttu-id="b7246-110">Para combinar albaranes</span><span class="sxs-lookup"><span data-stu-id="b7246-110">To combine receipts</span></span>  
1. <span data-ttu-id="b7246-111">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas compra** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="b7246-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b7246-112">Seleccione la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="b7246-112">Choose the **New** action.</span></span> <span data-ttu-id="b7246-113">Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="b7246-113">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>  
3. <span data-ttu-id="b7246-114">En la ficha desplegable Líneas, haga clic en **Acciones**, y elija la acción **Traer líns. recep**.</span><span class="sxs-lookup"><span data-stu-id="b7246-114">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span></span>  
4. <span data-ttu-id="b7246-115">Seleccione las distintas líneas de albarán que desee incluir en la factura.</span><span class="sxs-lookup"><span data-stu-id="b7246-115">Select multiple receipt lines that you want to include in the invoice.</span></span>  

    <span data-ttu-id="b7246-116">Si se ha seleccionado una línea de albarán incorrecta o desea comenzar desde el principio, simplemente elimine las líneas de la factura de compra y vuelva a usar la función **Traer líns. recep**.</span><span class="sxs-lookup"><span data-stu-id="b7246-116">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span></span>  
5. <span data-ttu-id="b7246-117">Para registrar la factura, elija la acción **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="b7246-117">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a><span data-ttu-id="b7246-118">Procedimiento para eliminar pedidos de compra abiertos después del registro de recepción combinada</span><span class="sxs-lookup"><span data-stu-id="b7246-118">To remove open purchase orders after combined receipt posting</span></span>  
1. <span data-ttu-id="b7246-119">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Eliminar peds. compra. factdos...** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="b7246-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span></span>  
2. <span data-ttu-id="b7246-120">Rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="b7246-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="b7246-121">.</span><span class="sxs-lookup"><span data-stu-id="b7246-121">.</span></span>
3. <span data-ttu-id="b7246-122">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="b7246-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="b7246-123">También puede eliminar los pedidos individuales manualmente.</span><span class="sxs-lookup"><span data-stu-id="b7246-123">Alternatively, delete the individual orders manually.</span></span>

<span data-ttu-id="b7246-124">Repita las tareas 1 a 3 para cualquier otro documento asignado, como pedidos abiertos de compra.</span><span class="sxs-lookup"><span data-stu-id="b7246-124">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="b7246-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="b7246-125">See Also</span></span>  
[<span data-ttu-id="b7246-126">Compras</span><span class="sxs-lookup"><span data-stu-id="b7246-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b7246-127">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b7246-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
