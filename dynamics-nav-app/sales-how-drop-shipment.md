---
title: "Procedimiento: Realizar envíos directos"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: es-es
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="4bdc1-102">Procedimiento: Realizar envíos directos</span><span class="sxs-lookup"><span data-stu-id="4bdc1-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="4bdc1-103">Un envío directo es el envío de los productos de uno de sus proveedores directamente a uno de sus clientes.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="4bdc1-104">Cuando marca un pedido de venta con el envío directo y crea un pedido especificando el cliente en el campo **Venta a-N.º cliente**</span><span class="sxs-lookup"><span data-stu-id="4bdc1-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="4bdc1-105">puede vincular los dos documentos y así asignar instrucciones al proveedor para que envíe el producto directamente al cliente.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="4bdc1-106">Para crear un pedido de venta de envío directo</span><span class="sxs-lookup"><span data-stu-id="4bdc1-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="4bdc1-107">Para preparar un envío directo cree un pedido de venta como si fuese normal, pero indique en la línea de ventas que dicha venta requiere un envío directo.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="4bdc1-108">Cree un pedido de ventas para un artículo.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-108">Create a sales order for an item.</span></span> <span data-ttu-id="4bdc1-109">Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="4bdc1-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="4bdc1-110">En la línea del pedido de venta del artículo con envío directo, seleccione la casilla **Envío directo**.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="4bdc1-111">Para crear pedidos de compra para envíos directos</span><span class="sxs-lookup"><span data-stu-id="4bdc1-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="4bdc1-112">Para preparar un envío directo de un producto que se va a vender, cree un pedido de compra como si fuese normal, pero indique en el pedido que el producto debe enviarse directamente al cliente no a usted.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="4bdc1-113">Cree un pedido de compra.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-113">Create a purchase order.</span></span> <span data-ttu-id="4bdc1-114">No rellene ningún campo en las líneas.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="4bdc1-115">Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="4bdc1-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="4bdc1-116">En el campo **Venta a-N.º cliente**,</span><span class="sxs-lookup"><span data-stu-id="4bdc1-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="4bdc1-117">seleccione el cliente al que le está vendiendo.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="4bdc1-118">Elija la acción **Envíos directos** y, a continuación, **Traer pedido venta**.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="4bdc1-119">En la ventana **Lista ventas**, seleccione el pedido de ventas que ha preparado en la sección "Para crear un pedido de venta de envío directo".</span><span class="sxs-lookup"><span data-stu-id="4bdc1-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="4bdc1-120">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-120">Choose the **OK** button.</span></span>

<span data-ttu-id="4bdc1-121">La información de la línea del pedido de venta se inserta en las líneas del pedido de compra.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="4bdc1-122">Ahora puede asignar instrucciones al proveedor para que envíe los productos al cliente, por ejemplo, enviando el pedido de compra por correo electrónico en formato PDF.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="4bdc1-123">Para ver el pedido de compra vinculado al pedido de venta.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="4bdc1-124">Seleccione la línea del envío directo del pedido de compra, elija las acciones **Pedido**, **Envío directo** y, a continuación, **Pedido de compra**.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="4bdc1-125">El pedido de compra vinculado se abre.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="4bdc1-126">Para registrar un envío directo</span><span class="sxs-lookup"><span data-stu-id="4bdc1-126">To post a drop shipment</span></span>
<span data-ttu-id="4bdc1-127">Cuando el proveedor ha enviado los artículos, puede establecer los pedidos de venta como enviados.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="4bdc1-128">También puede registrar el pedido de compra, pero solo con la opción **Recibir** hasta que se haya facturado el pedido de ventas.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="4bdc1-129">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Pedidos de ventas** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="4bdc1-130">Abra el pedido de venta que ha creado en la sección "Para crear un pedido de venta de envío directo".</span><span class="sxs-lookup"><span data-stu-id="4bdc1-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="4bdc1-131">En el campo **Cantidad a enviar**, especifiqué qué cantidad del pedido debe enviarse, todo o solo una parte.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="4bdc1-132">Seleccione la acción **Registrar** o **Registrar y enviar**.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="4bdc1-133">Elija la opción **Enviar** para facturar más adelante o la opción **Enviar y facturar** para facturar ahora.</span><span class="sxs-lookup"><span data-stu-id="4bdc1-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="4bdc1-134">Consulte también</span><span class="sxs-lookup"><span data-stu-id="4bdc1-134">See Also</span></span>
<span data-ttu-id="4bdc1-135">[Vender productos](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="4bdc1-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="4bdc1-136">Registro de compras</span><span class="sxs-lookup"><span data-stu-id="4bdc1-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="4bdc1-137">Gestionar ventas</span><span class="sxs-lookup"><span data-stu-id="4bdc1-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="4bdc1-138">[Gestionar inventario](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="4bdc1-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="4bdc1-139">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="4bdc1-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

