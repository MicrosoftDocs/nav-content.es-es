---
title: "Detalles de diseño: Registro de coste previsto"
description: "Los costes previstos representan la estimación, por ejemplo, del coste de un producto comprado registrado antes de recibir la factura de este producto."
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
ms.openlocfilehash: 0b14943e1bb214c26dfbae765a2467df1d06e50b
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-expected-cost-posting"></a><span data-ttu-id="d5ff6-103">Detalles de diseño: Registro de coste previsto</span><span class="sxs-lookup"><span data-stu-id="d5ff6-103">Design Details: Expected Cost Posting</span></span>
<span data-ttu-id="d5ff6-104">Los costes previstos representan la estimación, por ejemplo, del coste de un producto comprado registrado antes de recibir la factura de este producto.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span></span>  

 <span data-ttu-id="d5ff6-105">Puede registrar el coste previsto en el inventario y en la contabilidad.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-105">You can post expected cost to inventory and to the general ledger.</span></span> <span data-ttu-id="d5ff6-106">Cuando se registra una cantidad que solo se ha recibido o enviado, pero no se ha facturado, se crea un movimiento de valoración con el coste previsto.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span></span> <span data-ttu-id="d5ff6-107">Este coste previsto afecta al valor de inventario, pero no se registra en la contabilidad a no ser que se haya configurado el sistema para tal fin.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d5ff6-108">Los costes previstos solo se gestionan para transacciones de productos.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-108">Expected costs are only managed for item transactions.</span></span> <span data-ttu-id="d5ff6-109">Los costes previstos no son tipos de transacciones no materiales, como capacidad y cargos de productos.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-109">Expected costs are not for immaterial transaction types, such as capacity and item charges.</span></span>  

 <span data-ttu-id="d5ff6-110">Si solo se ha registrado la parte de la cantidad de una entrada de existencias, el valor de inventario en la contabilidad no cambia, a menos que haya seleccionado la casilla **Regis. cte. previsto en contab.** en la ventana **Configuración de inventario**.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box in the **Inventory Setup** window.</span></span> <span data-ttu-id="d5ff6-111">En ese caso, el coste previsto se registra en las cuentas provisionales en el momento de recepción.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span></span> <span data-ttu-id="d5ff6-112">Tras haber facturado por completo el albarán, las cuentas provisionales se saldan y el coste real se registra en la cuenta de inventario.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span></span>  

 <span data-ttu-id="d5ff6-113">Para respaldar el trabajo de conciliación y trazabilidad, el movimiento de valoración facturado muestra el importe del coste previsto que se ha registrado para cuadrar las cuentas provisionales.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span></span>  

## <a name="example"></a><span data-ttu-id="d5ff6-114">Ejemplo</span><span class="sxs-lookup"><span data-stu-id="d5ff6-114">Example</span></span>  
 <span data-ttu-id="d5ff6-115">En el ejemplo siguiente se muestra el coste previsto si las casillas **Variación existencias automát.** y **Regis. cte. previsto en contab.** se seleccionan en la ventana **Configuración de inventario**.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected in the **Inventory Setup** window.</span></span>  

 <span data-ttu-id="d5ff6-116">Registra un pedido de compra como recibido.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-116">You post a purchase order as received.</span></span> <span data-ttu-id="d5ff6-117">El coste previsto es de 95,00 DL.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-117">The expected cost is LCY 95.00.</span></span>  

 <span data-ttu-id="d5ff6-118">**Valor mov.**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-118">**Value Entries**</span></span>  

|<span data-ttu-id="d5ff6-119">Fecha registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-119">Posting Date</span></span>|<span data-ttu-id="d5ff6-120">Tipo mov.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-120">Entry Type</span></span>|<span data-ttu-id="d5ff6-121">Importe coste (Esperado)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-121">Cost Amount (Expected)</span></span>|<span data-ttu-id="d5ff6-122">Coste esperado reg. en cont.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-122">Expected Cost Posted to G/L</span></span>|<span data-ttu-id="d5ff6-123">Coste previsto</span><span class="sxs-lookup"><span data-stu-id="d5ff6-123">Expected Cost</span></span>|<span data-ttu-id="d5ff6-124">Nº mov. producto</span><span class="sxs-lookup"><span data-stu-id="d5ff6-124">Item Ledger Entry No.</span></span>|<span data-ttu-id="d5ff6-125">Nº mov.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-125">Entry No.</span></span>|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="d5ff6-126">01-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-126">01-01-20</span></span>|<span data-ttu-id="d5ff6-127">Coste directo</span><span class="sxs-lookup"><span data-stu-id="d5ff6-127">Direct Cost</span></span>|<span data-ttu-id="d5ff6-128">95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-128">95.00</span></span>|<span data-ttu-id="d5ff6-129">95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-129">95.00</span></span>|<span data-ttu-id="d5ff6-130">Sí</span><span class="sxs-lookup"><span data-stu-id="d5ff6-130">Yes</span></span>|<span data-ttu-id="d5ff6-131">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-131">1</span></span>|<span data-ttu-id="d5ff6-132">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-132">1</span></span>|  

 <span data-ttu-id="d5ff6-133">**Movimientos de relación en C/G: tabla Relación movs. productos**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="d5ff6-134">Nº mov. contabilidad</span><span class="sxs-lookup"><span data-stu-id="d5ff6-134">G/L Entry No.</span></span>|<span data-ttu-id="d5ff6-135">Nº mov. valor</span><span class="sxs-lookup"><span data-stu-id="d5ff6-135">Value Entry No.</span></span>|<span data-ttu-id="d5ff6-136">Nº asto. registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-136">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="d5ff6-137">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-137">1</span></span>|<span data-ttu-id="d5ff6-138">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-138">1</span></span>|<span data-ttu-id="d5ff6-139">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-139">1</span></span>|  
|<span data-ttu-id="d5ff6-140">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-140">2</span></span>|<span data-ttu-id="d5ff6-141">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-141">1</span></span>|<span data-ttu-id="d5ff6-142">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-142">1</span></span>|  

 <span data-ttu-id="d5ff6-143">**Movs. contabilidad**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-143">**General Ledger Entries**</span></span>  

|<span data-ttu-id="d5ff6-144">Fecha registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-144">Posting Date</span></span>|<span data-ttu-id="d5ff6-145">Cuenta</span><span class="sxs-lookup"><span data-stu-id="d5ff6-145">G/L Account</span></span>|<span data-ttu-id="d5ff6-146">Nº cuenta (demostración En-US)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-146">Account No. (En-US Demo)</span></span>|<span data-ttu-id="d5ff6-147">Importe</span><span class="sxs-lookup"><span data-stu-id="d5ff6-147">Amount</span></span>|<span data-ttu-id="d5ff6-148">Nº mov.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-148">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="d5ff6-149">01-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-149">01-01-20</span></span>|<span data-ttu-id="d5ff6-150">Cuenta de ajuste de inventario (provisional)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-150">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="d5ff6-151">5530</span><span class="sxs-lookup"><span data-stu-id="d5ff6-151">5530</span></span>|<span data-ttu-id="d5ff6-152">-95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-152">-95.00</span></span>|<span data-ttu-id="d5ff6-153">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-153">2</span></span>|  
|<span data-ttu-id="d5ff6-154">01-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-154">01-01-20</span></span>|<span data-ttu-id="d5ff6-155">Cta. inventario (provisional)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-155">Inventory Account (Interim)</span></span>|<span data-ttu-id="d5ff6-156">2131</span><span class="sxs-lookup"><span data-stu-id="d5ff6-156">2131</span></span>|<span data-ttu-id="d5ff6-157">95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-157">95.00</span></span>|<span data-ttu-id="d5ff6-158">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-158">1</span></span>|  

 <span data-ttu-id="d5ff6-159">En una fecha posterior, el pedido de compra se puede registrar como facturado.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-159">At a later date, you post the purchase order as invoiced.</span></span> <span data-ttu-id="d5ff6-160">El coste facturado es de 100,00 DL.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-160">The invoiced cost is LCY 100.00.</span></span>  

 <span data-ttu-id="d5ff6-161">**Valor mov.**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-161">**Value Entries**</span></span>  

|<span data-ttu-id="d5ff6-162">Fecha registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-162">Posting Date</span></span>|<span data-ttu-id="d5ff6-163">Importe coste (Real)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-163">Cost Amount (Actual)</span></span>|<span data-ttu-id="d5ff6-164">Importe coste (Esperado)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-164">Cost Amount (Expected)</span></span>|<span data-ttu-id="d5ff6-165">Coste regis. en contab.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-165">Cost Posted to G/L</span></span>|<span data-ttu-id="d5ff6-166">Coste previsto</span><span class="sxs-lookup"><span data-stu-id="d5ff6-166">Expected Cost</span></span>|<span data-ttu-id="d5ff6-167">Nº mov. producto</span><span class="sxs-lookup"><span data-stu-id="d5ff6-167">Item Ledger Entry No.</span></span>|<span data-ttu-id="d5ff6-168">Nº mov.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-168">Entry No.</span></span>|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="d5ff6-169">15-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-169">01-15-20</span></span>|<span data-ttu-id="d5ff6-170">100.00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-170">100.00</span></span>|<span data-ttu-id="d5ff6-171">-95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-171">-95.00</span></span>|<span data-ttu-id="d5ff6-172">100.00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-172">100.00</span></span>|<span data-ttu-id="d5ff6-173">No</span><span class="sxs-lookup"><span data-stu-id="d5ff6-173">No</span></span>|<span data-ttu-id="d5ff6-174">1</span><span class="sxs-lookup"><span data-stu-id="d5ff6-174">1</span></span>|<span data-ttu-id="d5ff6-175">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-175">2</span></span>|  

 <span data-ttu-id="d5ff6-176">**Movimientos de relación en C/G: tabla Relación movs. productos**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="d5ff6-177">Nº mov. contabilidad</span><span class="sxs-lookup"><span data-stu-id="d5ff6-177">G/L Entry No.</span></span>|<span data-ttu-id="d5ff6-178">Nº mov. valor</span><span class="sxs-lookup"><span data-stu-id="d5ff6-178">Value Entry No.</span></span>|<span data-ttu-id="d5ff6-179">Nº asto. registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-179">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="d5ff6-180">3</span><span class="sxs-lookup"><span data-stu-id="d5ff6-180">3</span></span>|<span data-ttu-id="d5ff6-181">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-181">2</span></span>|<span data-ttu-id="d5ff6-182">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-182">2</span></span>|  
|<span data-ttu-id="d5ff6-183">4</span><span class="sxs-lookup"><span data-stu-id="d5ff6-183">4</span></span>|<span data-ttu-id="d5ff6-184">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-184">2</span></span>|<span data-ttu-id="d5ff6-185">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-185">2</span></span>|  
|<span data-ttu-id="d5ff6-186">5</span><span class="sxs-lookup"><span data-stu-id="d5ff6-186">5</span></span>|<span data-ttu-id="d5ff6-187">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-187">2</span></span>|<span data-ttu-id="d5ff6-188">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-188">2</span></span>|  
|<span data-ttu-id="d5ff6-189">6</span><span class="sxs-lookup"><span data-stu-id="d5ff6-189">6</span></span>|<span data-ttu-id="d5ff6-190">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-190">2</span></span>|<span data-ttu-id="d5ff6-191">2</span><span class="sxs-lookup"><span data-stu-id="d5ff6-191">2</span></span>|  

 <span data-ttu-id="d5ff6-192">**Movs. contabilidad**</span><span class="sxs-lookup"><span data-stu-id="d5ff6-192">**General Ledger Entries**</span></span>  

|<span data-ttu-id="d5ff6-193">Fecha registro</span><span class="sxs-lookup"><span data-stu-id="d5ff6-193">Posting Date</span></span>|<span data-ttu-id="d5ff6-194">Cuenta</span><span class="sxs-lookup"><span data-stu-id="d5ff6-194">G/L Account</span></span>|<span data-ttu-id="d5ff6-195">Nº cuenta (demostración En-US)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-195">Account No. (En-US Demo)</span></span>|<span data-ttu-id="d5ff6-196">Importe</span><span class="sxs-lookup"><span data-stu-id="d5ff6-196">Amount</span></span>|<span data-ttu-id="d5ff6-197">Nº mov.</span><span class="sxs-lookup"><span data-stu-id="d5ff6-197">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="d5ff6-198">15-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-198">01-15-20</span></span>|<span data-ttu-id="d5ff6-199">Cuenta de ajuste de inventario (provisional)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-199">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="d5ff6-200">5530</span><span class="sxs-lookup"><span data-stu-id="d5ff6-200">5530</span></span>|<span data-ttu-id="d5ff6-201">95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-201">95.00</span></span>|<span data-ttu-id="d5ff6-202">4</span><span class="sxs-lookup"><span data-stu-id="d5ff6-202">4</span></span>|  
|<span data-ttu-id="d5ff6-203">15-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-203">01-15-20</span></span>|<span data-ttu-id="d5ff6-204">Cta. inventario (provisional)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-204">Inventory Account (Interim)</span></span>|<span data-ttu-id="d5ff6-205">2131</span><span class="sxs-lookup"><span data-stu-id="d5ff6-205">2131</span></span>|<span data-ttu-id="d5ff6-206">-95,00</span><span class="sxs-lookup"><span data-stu-id="d5ff6-206">-95.00</span></span>|<span data-ttu-id="d5ff6-207">3</span><span class="sxs-lookup"><span data-stu-id="d5ff6-207">3</span></span>|  
|<span data-ttu-id="d5ff6-208">15-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-208">01-15-20</span></span>|<span data-ttu-id="d5ff6-209">Cuenta aplic. coste directo</span><span class="sxs-lookup"><span data-stu-id="d5ff6-209">Direct Cost Applied Account</span></span>|<span data-ttu-id="d5ff6-210">7291</span><span class="sxs-lookup"><span data-stu-id="d5ff6-210">7291</span></span>|<span data-ttu-id="d5ff6-211">-100</span><span class="sxs-lookup"><span data-stu-id="d5ff6-211">-100</span></span>|<span data-ttu-id="d5ff6-212">6</span><span class="sxs-lookup"><span data-stu-id="d5ff6-212">6</span></span>|  
|<span data-ttu-id="d5ff6-213">15-01-20</span><span class="sxs-lookup"><span data-stu-id="d5ff6-213">01-15-20</span></span>|<span data-ttu-id="d5ff6-214">Cta. inventario</span><span class="sxs-lookup"><span data-stu-id="d5ff6-214">Inventory Account</span></span>|<span data-ttu-id="d5ff6-215">2130</span><span class="sxs-lookup"><span data-stu-id="d5ff6-215">2130</span></span>|<span data-ttu-id="d5ff6-216">100</span><span class="sxs-lookup"><span data-stu-id="d5ff6-216">100</span></span>|<span data-ttu-id="d5ff6-217">5</span><span class="sxs-lookup"><span data-stu-id="d5ff6-217">5</span></span>|  

## <a name="see-also"></a><span data-ttu-id="d5ff6-218">Consulte también</span><span class="sxs-lookup"><span data-stu-id="d5ff6-218">See Also</span></span>
 <span data-ttu-id="d5ff6-219">[Detalles de diseño: Coste de inventario](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="d5ff6-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="d5ff6-220">[Detalles de diseño: Ajuste de coste](design-details-cost-adjustment.md) </span><span class="sxs-lookup"><span data-stu-id="d5ff6-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span></span>  
 <span data-ttu-id="d5ff6-221">[Detalles de diseño: Conciliación con contabilidad](design-details-reconciliation-with-the-general-ledger.md) </span><span class="sxs-lookup"><span data-stu-id="d5ff6-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span></span>  
 <span data-ttu-id="d5ff6-222">[Detalles de diseño: Registro de inventario](design-details-inventory-posting.md) </span><span class="sxs-lookup"><span data-stu-id="d5ff6-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span></span>  
 [<span data-ttu-id="d5ff6-223">Detalles de diseño: Desviación</span><span class="sxs-lookup"><span data-stu-id="d5ff6-223">Design Details: Variance</span></span>](design-details-variance.md)  
 [<span data-ttu-id="d5ff6-224">Gestión de costes de inventario</span><span class="sxs-lookup"><span data-stu-id="d5ff6-224">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="d5ff6-225">Finanzas</span><span class="sxs-lookup"><span data-stu-id="d5ff6-225">Finance</span></span>](finance.md)  
 <span data-ttu-id="d5ff6-226">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d5ff6-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
