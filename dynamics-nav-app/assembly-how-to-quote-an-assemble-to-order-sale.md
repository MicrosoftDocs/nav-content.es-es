---
title: Oferta de una venta de ensamblar para pedido
description: "Puede utilizar la administración de ensamblados para personalizar un artículo del ensamblado a la solicitud de un cliente durante el proceso de venta."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ee62ddff43778bd81d4ed65c2dcdd466b79e422
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a><span data-ttu-id="7dee8-103">Procedimiento: Oferta de una venta de ensamblar para pedido</span><span class="sxs-lookup"><span data-stu-id="7dee8-103">How to: Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="7dee8-104">Puede utilizar la administración de ensamblados para personalizar un artículo del ensamblado a la solicitud de un cliente durante el proceso de venta.</span><span class="sxs-lookup"><span data-stu-id="7dee8-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="7dee8-105">Para obtener más información, consulte [Procedimiento: Venta de artículos ensamblados para pedido](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="7dee8-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="7dee8-106">Como cuando se vende cualquier otro tipo de producto, también puede crear una oferta de venta para un elemento del ensamblado personalizado antes de convertirlo en un pedido de venta.</span><span class="sxs-lookup"><span data-stu-id="7dee8-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="7dee8-107">Este proceso implica varios pasos adicionales cuando se compara con crear una oferta de venta regular y usa una variación de un pedido de ensamblado vinculado, que es una oferta de ensamblado.</span><span class="sxs-lookup"><span data-stu-id="7dee8-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="7dee8-108">Como todos los tipos de oferta, las cantidades en ofertas de ensamblado no se utilizan en la disponibilidad, la planificación o las reservas.</span><span class="sxs-lookup"><span data-stu-id="7dee8-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="7dee8-109">Para crear una oferta de venta de productos ensamblar para pedido</span><span class="sxs-lookup"><span data-stu-id="7dee8-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="7dee8-110">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Oferta de venta** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="7dee8-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7dee8-111">Cree una línea de oferta de venta con una línea para un elemento del ensamblado.</span><span class="sxs-lookup"><span data-stu-id="7dee8-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="7dee8-112">Para obtener más información, vea [Procedimiento: Realización de ofertas](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="7dee8-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="7dee8-113">En el campo **Cdad. al ensamblar para pedido**, introduzca la cantidad total.</span><span class="sxs-lookup"><span data-stu-id="7dee8-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="7dee8-114">No debe crear una oferta para una cantidad parcial.</span><span class="sxs-lookup"><span data-stu-id="7dee8-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="7dee8-115">Por tanto, deberá introducir la misma cantidad que ha introducido en el campo **Cantidad** de la línea de oferta de venta.</span><span class="sxs-lookup"><span data-stu-id="7dee8-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="7dee8-116">En la ficha desplegable **Líneas**, seleccione **Línea**, seleccione **Ensamblar para pedido** y, a continuación, elija **Ensamblar para líneas de pedido**.</span><span class="sxs-lookup"><span data-stu-id="7dee8-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="7dee8-117">También puede elegir el campo **Cdad. al ensamblar para pedido** en la línea.</span><span class="sxs-lookup"><span data-stu-id="7dee8-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="7dee8-118">En la ventana **Ensamblar para líneas de pedido**, revise o modifique las líneas de pedido de ensamblado de acuerdo con la oferta que el cliente solicita.</span><span class="sxs-lookup"><span data-stu-id="7dee8-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="7dee8-119">Si desea ver más información, seleccione la acción **Mostrar documento** para abrir el pedido de oferta abierto completo.</span><span class="sxs-lookup"><span data-stu-id="7dee8-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="7dee8-120">No puede modificar el contenido de la mayoría de los campos, y no puede realizar ningún registro.</span><span class="sxs-lookup"><span data-stu-id="7dee8-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="7dee8-121">Cuando se hayan ajustado las líneas del pedido de ensamblado a la oferta, cierre la ventana **Ensamblar para líneas de pedido** para volver a la ventana **Oferta venta**.</span><span class="sxs-lookup"><span data-stu-id="7dee8-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="7dee8-122">Si el cliente acepta la oferta, cree un pedido de venta para el elemento del ensamblado ofertado.</span><span class="sxs-lookup"><span data-stu-id="7dee8-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="7dee8-123">Para obtener más información, vea [Procedimiento: Realización de ofertas](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="7dee8-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="7dee8-124">La oferta de ensamblado vinculada y cualquier personalización se asocian a ese nuevo pedido de venta para preparar el ensamblado del producto o los productos que se van a vender.</span><span class="sxs-lookup"><span data-stu-id="7dee8-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7dee8-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="7dee8-125">See Also</span></span>  
[<span data-ttu-id="7dee8-126">Gestión de ensamblaje</span><span class="sxs-lookup"><span data-stu-id="7dee8-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="7dee8-127">Trabajar con listas de materiales</span><span class="sxs-lookup"><span data-stu-id="7dee8-127">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="7dee8-128">Grupos contables inventario</span><span class="sxs-lookup"><span data-stu-id="7dee8-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="7dee8-129">Detalles de diseño: Gestión de almacén</span><span class="sxs-lookup"><span data-stu-id="7dee8-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="7dee8-130">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7dee8-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
