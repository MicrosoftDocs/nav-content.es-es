---
title: Procedimiento para eliminar movimientos de presupuestos de costes
description: Utilice el trabajo por lotes **Eliminar movimientos presupuesto de costes** para anular los movimientos de presupuesto de costes del registro de presupuestos de costes.
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
ms.openlocfilehash: 16c471b7c03d8b53049ad2284dbe4fa058dd3ca9
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-delete-cost-budget-entries"></a><span data-ttu-id="f9844-103">Procedimiento para eliminar movimientos de presupuestos de costes</span><span class="sxs-lookup"><span data-stu-id="f9844-103">How to: Delete Cost Budget Entries</span></span>
<span data-ttu-id="f9844-104">Utilice el trabajo por lotes **Eliminar movimientos presupuesto de costes** para anular los movimientos de presupuesto de costes del registro de presupuestos de costes.</span><span class="sxs-lookup"><span data-stu-id="f9844-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="f9844-105">Para evitar cualquier discontinuidad en movimientos de presupuesto de costes y movimientos de registro de costes, no puede eliminar un único movimiento o sección de movimientos del centro de la lista de los movimientos de registro.</span><span class="sxs-lookup"><span data-stu-id="f9844-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="f9844-106">Para eliminar movimientos de presupuesto de costes</span><span class="sxs-lookup"><span data-stu-id="f9844-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="f9844-107">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Eliminar movs. ppto. costes** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="f9844-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="f9844-108">El campo **Hasta nº registro**</span><span class="sxs-lookup"><span data-stu-id="f9844-108">The **To Register No.**</span></span> <span data-ttu-id="f9844-109">contiene siempre el último número de movimiento de registro, que no se puede cambiar.</span><span class="sxs-lookup"><span data-stu-id="f9844-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="f9844-110">Puede usar el campo **Desde nº registro**</span><span class="sxs-lookup"><span data-stu-id="f9844-110">You can use the **From Register No.**</span></span> <span data-ttu-id="f9844-111">para seleccionar un número de movimiento de registro del que debe iniciar la eliminación.</span><span class="sxs-lookup"><span data-stu-id="f9844-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="f9844-112">Elija el botón **ACEPTAR** para eliminar los movimientos de presupuestos de costes seleccionados.</span><span class="sxs-lookup"><span data-stu-id="f9844-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f9844-113">Para evitar una eliminación accidental de los movimientos de presupuesto de coste, puede cerrar movimientos de registro marcando las líneas como **Cerrado** en el campo **Cerrado** en la ventana **Registro de presupuesto de costes**.</span><span class="sxs-lookup"><span data-stu-id="f9844-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field in the **Cost Budget Registers** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f9844-114">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f9844-114">See Also</span></span>  
<span data-ttu-id="f9844-115">[Contabilidad para costes](finance-manage-cost-accounting.md)
[Crear presupuesto coste](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="f9844-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="f9844-116">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f9844-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
