---
title: Asignar cargos de producto a ventas y compras
description: "Si desea que sus productos de inventario carguen costes adicionales, tales como fletes, manipulación física, seguros y transporte en los que incurra al comprar o vender artículos, puede usar la función Gastos de productos."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: transportation, added cost
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f5eebe7d1837657771d4f3004627be716d4d51bc
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-use-item-charges-to-account-for-additional-trade-costs"></a><span data-ttu-id="cec6e-103">Utilizar los cargos de producto a cuenta para los costes comerciales adicionales</span><span class="sxs-lookup"><span data-stu-id="cec6e-103">How to: Use Item Charges to Account for Additional Trade Costs</span></span>
<span data-ttu-id="cec6e-104">Para asegurarse de la valoración correcta, sus productos de inventario deben cargar costes adicionales, tales como fletes, manipulación física, seguros y transporte en los que incurra al comprar o vender artículos.</span><span class="sxs-lookup"><span data-stu-id="cec6e-104">To ensure correct valuation, your inventory items must carry any added costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing or selling the items.</span></span> <span data-ttu-id="cec6e-105">Para las compras, el coste de descarga de un producto comprado se compone del precio de compra del proveedor sumado a todos los cargos de producto directos adicionales que se pueden asignar a albaranes o envíos devueltos determinados.</span><span class="sxs-lookup"><span data-stu-id="cec6e-105">For purchases, the landed cost of a purchased item consists of the vendor's purchase price and all additional direct item charges that can be assigned to individual receipts or return shipments.</span></span> <span data-ttu-id="cec6e-106">Para las compras, conocer el coste de envío de los productos vendidos es tan importante para la empresa como conocer el coste de los productos comprados.</span><span class="sxs-lookup"><span data-stu-id="cec6e-106">For sales, knowing the cost of shipping sold items can be as vital to your company as knowing the landed cost of purchased items.</span></span>

<span data-ttu-id="cec6e-107">Además de registrar el coste añadido en el valor de inventario, puede usar la función de cargos de producto para:</span><span class="sxs-lookup"><span data-stu-id="cec6e-107">In addition to recording the added cost in you inventory value, you can use the Item Charges feature for the following:</span></span>

- <span data-ttu-id="cec6e-108">Identificar el coste de descarga de un producto para tomar decisiones exactas sobre cómo optimizar la red de distribución.</span><span class="sxs-lookup"><span data-stu-id="cec6e-108">Identify the landed cost of an item for making more accurate decisions on how to optimize the distribution network.</span></span>
- <span data-ttu-id="cec6e-109">Desglosar el coste unitario o el precio de venta de un producto con fines de análisis.</span><span class="sxs-lookup"><span data-stu-id="cec6e-109">Break down the unit cost or unit price of an item for analysis purposes.</span></span>
- <span data-ttu-id="cec6e-110">Incluir las deducciones de compras en el coste unitario y las deducciones de ventas en el precio de venta.</span><span class="sxs-lookup"><span data-stu-id="cec6e-110">include purchase allowances into the unit cost and sales allowances into the unit price.</span></span>

<span data-ttu-id="cec6e-111">Antes de poder asignar cargos por productos, debe configurar los números de cargos de productos para los diferentes tipos de cargos de productos, incluyendo los costes de cuentas de contables relacionados con ventas, compras y ajustes de inventario.</span><span class="sxs-lookup"><span data-stu-id="cec6e-111">Before you can assign item charges, you must set up item charge numbers for the different types of item charges, including to which G/L accounts costs related to sales, purchases, and inventory adjustments are posted to.</span></span> <span data-ttu-id="cec6e-112">Un número de cargo de producto contiene una combinación de grupo contable de producto, código de grupo de impuesto, grupo de registro IVA producto y cargos de producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-112">An item charge number contains a combination of general product posting group, tax group code, VAT product posting group, and item charge.</span></span> <span data-ttu-id="cec6e-113">Al introducir el número de coste de producto en un documento de compra o de venta, se obtendrá una cuenta según la configuración del número de coste de producto y la información almacenada en el documento.</span><span class="sxs-lookup"><span data-stu-id="cec6e-113">When you enter the item charge number on a purchase or sales document, the relevant G/L account is retrieved based on the setup of the item charge number and the information on the document.</span></span>

<span data-ttu-id="cec6e-114">Para los documentos de compra y de venta, puede asignar un coste de producto de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="cec6e-114">For both purchase and sales documents, you can assign an item charge in two ways:</span></span>
- <span data-ttu-id="cec6e-115">en el documento donde están registrados los productos a los que se refiere el cargo de producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-115">On the document where the items that the item charge relates to are listed.</span></span> <span data-ttu-id="cec6e-116">Esto se suele hacer para los documentos que aún no se han publicado completamente.</span><span class="sxs-lookup"><span data-stu-id="cec6e-116">This you typically do for documents that are not yet fully posted.</span></span>
- <span data-ttu-id="cec6e-117">en una factura independiente asociando el cargo de producto a envíos o albaranes registrados en los que figuran los productos a los que se refiere el cargo de producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-117">On a separate invoice by linking the item charge to a posted receipt or shipment where the items that the item charge relate to are listed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="cec6e-118">Puede asignar cargos de artículos a pedidos, facturas y abonos para ventas y compras.</span><span class="sxs-lookup"><span data-stu-id="cec6e-118">You can assign item charges to orders, invoices, and credit memos, for both sales and purchases.</span></span> <span data-ttu-id="cec6e-119">Los procedimientos siguientes describen cómo gestionar los cargos de producto en una factura de compra.</span><span class="sxs-lookup"><span data-stu-id="cec6e-119">The following procedures describe how to work with item charges for a purchase invoice.</span></span> <span data-ttu-id="cec6e-120">Los pasos son parecidos a los de los documentos de compra y venta.</span><span class="sxs-lookup"><span data-stu-id="cec6e-120">The steps are similar for all other purchase and sales documents.</span></span>

## <a name="to-set-up-item-charge-numbers"></a><span data-ttu-id="cec6e-121">Configurar números de coste de producto</span><span class="sxs-lookup"><span data-stu-id="cec6e-121">To set up item charge numbers</span></span>
<span data-ttu-id="cec6e-122">Los números de cargo de producto sirven para diferenciar los distintos tipos de cargos que se utilizan en la empresa.</span><span class="sxs-lookup"><span data-stu-id="cec6e-122">You use item charge numbers to distinguish between the different kinds of item charges that are used in your company.</span></span>

1. <span data-ttu-id="cec6e-123">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cargos producto** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="cec6e-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Charges**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec6e-124">En la ventana **Cargos producto**, seleccione la acción **Nuevo** para crear una línea nueva.</span><span class="sxs-lookup"><span data-stu-id="cec6e-124">In the **Item Charges** window, choose the **New** action to create a new line.</span></span>
3. <span data-ttu-id="cec6e-125">Rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="cec6e-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-an-item-charge-directly-to-the-purchase-invoice-for-the-item"></a><span data-ttu-id="cec6e-126">Asignar un coste de producto directamente en la factura de compra del producto</span><span class="sxs-lookup"><span data-stu-id="cec6e-126">To assign an item charge directly to the purchase invoice for the item</span></span>
<span data-ttu-id="cec6e-127">Si conoce el coste de un producto en el momento en que registra la factura de compra, siga este procedimiento.</span><span class="sxs-lookup"><span data-stu-id="cec6e-127">If you know the item charge at the time when you post a purchase invoice for the item, follow this procedure.</span></span>

1. <span data-ttu-id="cec6e-128">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas compra** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="cec6e-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec6e-129">Cree una nueva factura de compra.</span><span class="sxs-lookup"><span data-stu-id="cec6e-129">Create a new purchase invoice.</span></span> <span data-ttu-id="cec6e-130">Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="cec6e-130">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="cec6e-131">Asegúrese de que la factura de compra tiene una o más líneas del tipo Producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-131">Make sure the purchase invoice has one or more lines of type Item.</span></span>
4. <span data-ttu-id="cec6e-132">En una línea nueva, en el campo **Tipo**, seleccione **Cargo (prod.)**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-132">On a new line, in the **Type** field, select **Charge (Item)**.</span></span>
5. <span data-ttu-id="cec6e-133">En el campo **Cantidad**, introduzca las unidades del coste de producto que se han facturado.</span><span class="sxs-lookup"><span data-stu-id="cec6e-133">In the **Quantity** field, enter the units of the item charge that you have been invoiced for.</span></span>
6. <span data-ttu-id="cec6e-134">En el campo **Precio compra**, introduzca el importe del cargo de producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-134">In the **Direct Unit Cost** field, enter the amount of the item charge.</span></span>
7. <span data-ttu-id="cec6e-135">Rellene los campos restantes según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="cec6e-135">Fill in the remaining fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    <span data-ttu-id="cec6e-136">En los siguientes pasos, se efectuará la asignación actual.</span><span class="sxs-lookup"><span data-stu-id="cec6e-136">In the following steps, you will perform the actual assignment.</span></span> <span data-ttu-id="cec6e-137">Hasta que el cargo del producto esté completamente asignado, el valor en el campo **Cdad. para asignar** aparece de color rojo.</span><span class="sxs-lookup"><span data-stu-id="cec6e-137">Until the item charge is fully assigned, the value in the **Qty. to Assign** field is in red font.</span></span>
8. <span data-ttu-id="cec6e-138">En la ficha **Líneas**, seleccione la acción **Asignación cargo prod.**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-138">On the **Lines** tab, choose the **Item Charge Assignment** action.</span></span>

    <span data-ttu-id="cec6e-139">La ventana **Asignación cargos prod.** abre una línea por cada línea del tipo Producto en la factura de compra.</span><span class="sxs-lookup"><span data-stu-id="cec6e-139">The **Item Charge Assignment** window opens showing one line for each line of type Item on the purchase invoice.</span></span> <span data-ttu-id="cec6e-140">Para asignar el cargo de producto a una o más líneas de factura, puede utilizar una función que lo asigne y distribuya automáticamente o puede rellenar manualmente el campo **Cdad. para asignar**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-140">To assign the item charge to one or more invoice lines, you can use a function that assigns and distributes it for you or you can manually fill in the **Qty. to Assign** field.</span></span> <span data-ttu-id="cec6e-141">Las siguientes tareas describen cómo utilizar la funcionalidad de la asignación de cargos de producto el menú.</span><span class="sxs-lookup"><span data-stu-id="cec6e-141">The following steps describe how to use the Suggest Item Charge Assignment function.</span></span>

9. <span data-ttu-id="cec6e-142">En la ventana **Asignación cargos prod.**, seleccione la acción **Sugerir asignación cargo prod.**</span><span class="sxs-lookup"><span data-stu-id="cec6e-142">In the **Item Charge Assignment** window, choose the **Suggest Item Charge Assignment** action.</span></span>
10. <span data-ttu-id="cec6e-143">Si hay más de una línea de factura del tipo Producto, elija una de las cuatro opciones de distribución.</span><span class="sxs-lookup"><span data-stu-id="cec6e-143">If there are more than one invoice lines of type Item, choose one of the four distribution options.</span></span>  

<span data-ttu-id="cec6e-144">El cargo del producto está completamente asignado, el valor de la factura de compra en el campo **Cdad. para asignar** es cero.</span><span class="sxs-lookup"><span data-stu-id="cec6e-144">It the item charge is fully assigned, the value in the **Qty. to Assign** field on the purchase invoice is zero.</span></span>

<span data-ttu-id="cec6e-145">El cargo de producto está asignado a la factura de compra.</span><span class="sxs-lookup"><span data-stu-id="cec6e-145">The item charge is now assigned to the purchase invoice.</span></span> <span data-ttu-id="cec6e-146">Al registrar la recepción de la factura de compra, los valores de inventario de los elementos se actualizan con el coste del cargo del producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-146">When you post the receipt of the purchase invoice, the items' inventory values are updated with the cost of the item charge.</span></span>  

## <a name="to-assign-an-item-charge-from-a-separate-invoice-to-the-purchase-invoice-for-the-item"></a><span data-ttu-id="cec6e-147">Asignar un coste de producto de una factura independiente a la factura de compra del producto</span><span class="sxs-lookup"><span data-stu-id="cec6e-147">To assign an item charge from a separate invoice to the purchase invoice for the item</span></span>
<span data-ttu-id="cec6e-148">Si recibió una factura por el cargo de producto después de haber publicado el recibo de compra original, siga este procedimiento.</span><span class="sxs-lookup"><span data-stu-id="cec6e-148">If you received an invoice for the item charge after you posted the original purchase receipt, follow this procedure.</span></span>
1. <span data-ttu-id="cec6e-149">Repita los pasos del 1 al 8 en la sección "Asignar un coste de producto directamente en la factura de compra del producto".</span><span class="sxs-lookup"><span data-stu-id="cec6e-149">Repeat steps 1 through 8 in the "To assign an item charge directly to the purchase invoice for the item" section.</span></span>
2. <span data-ttu-id="cec6e-150">En la ventana **Asignación cargos prod.**, elija la acción **Traer líns. albarán**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-150">In the **Item Charge Assignment** window, choose the **Get Receipt Lines** action.</span></span>
3. <span data-ttu-id="cec6e-151">En la ventana **Líns. recep. compra**, seleccione el albarán de compra registrado para el producto al que desea asignar el cargo de producto y, a continuación, elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-151">In the **Purch. Receipt Lines** window, select the posted purchase receipt for the item that you want to assign the item charge to, and then choose the **OK** button.</span></span>
4. <span data-ttu-id="cec6e-152">Seleccione la acción **Sugerir asignación cargo prod.**</span><span class="sxs-lookup"><span data-stu-id="cec6e-152">Choose the **Suggest Item Charge Assignment** action.</span></span>

<span data-ttu-id="cec6e-153">El cargo de producto de la factura de compra independiente se asigna al producto en el recibo de compra registrado, y se actualiza el valor de inventario del artículo con el coste del cargo de producto.</span><span class="sxs-lookup"><span data-stu-id="cec6e-153">The item charge on the separate purchase invoice is now assigned to the item on the posted purchase receipt, thereby updating the item's inventory value with the cost of the item charge.</span></span>

## <a name="see-also"></a><span data-ttu-id="cec6e-154">Consulte también</span><span class="sxs-lookup"><span data-stu-id="cec6e-154">See Also</span></span>
[<span data-ttu-id="cec6e-155">Administrar pagos</span><span class="sxs-lookup"><span data-stu-id="cec6e-155">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="cec6e-156">Registro de compras</span><span class="sxs-lookup"><span data-stu-id="cec6e-156">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="cec6e-157">Facturación de ventas</span><span class="sxs-lookup"><span data-stu-id="cec6e-157">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
<span data-ttu-id="cec6e-158">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cec6e-158">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
