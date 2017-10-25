---
title: "Configuración y asiento de la regularización"
description: "Puede utilizar cuentas de regularización para saldar y realizar el seguimiento de varias cuentas al mismo tiempo. El proceso **Asiento regularización** transfiere las cuentas de regularización a una cuenta del balance y las cierra. Cuando se ejecuta el proceso **Asiento regularización**, los movimientos se registran automáticamente."
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
ms.openlocfilehash: 83031b5e8cbce289ecfba2d7fcb3a14b01642911
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-and-close-income-statement-balances"></a><span data-ttu-id="6e1da-105">Configuración y asiento de la regularización</span><span class="sxs-lookup"><span data-stu-id="6e1da-105">How to: Set Up and Close Income Statement Balances</span></span>
<span data-ttu-id="6e1da-106">Puede utilizar cuentas de regularización para saldar y realizar el seguimiento de varias cuentas al mismo tiempo.</span><span class="sxs-lookup"><span data-stu-id="6e1da-106">You can use income statement balancing accounts to balance and track several accounts at the same time.</span></span> <span data-ttu-id="6e1da-107">El proceso **Asiento regularización** transfiere las cuentas de regularización a una cuenta del balance y las cierra.</span><span class="sxs-lookup"><span data-stu-id="6e1da-107">The **Close Income Statement** batch job transfers income statement accounts to an account in the balance sheet, and closes the income statement accounts.</span></span> <span data-ttu-id="6e1da-108">Cuando se ejecuta el proceso **Asiento regularización**, los movimientos se registran automáticamente.</span><span class="sxs-lookup"><span data-stu-id="6e1da-108">When the **Close Income Statement** batch job is run, the entries are automatically posted.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="6e1da-109">Antes de ejecutar el proceso, se debe cerrar el ejercicio.</span><span class="sxs-lookup"><span data-stu-id="6e1da-109">The fiscal year must be closed before the batch job can run.</span></span>  
  
### <a name="to-set-up-the-income-statement-balance-account"></a><span data-ttu-id="6e1da-110">Para configurar la cuenta de regularización</span><span class="sxs-lookup"><span data-stu-id="6e1da-110">To set up the income statement balance account</span></span>  
  
1.  <span data-ttu-id="6e1da-111">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan de cuentas** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="6e1da-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="6e1da-112">Seleccione una cuenta de contabilidad existente.</span><span class="sxs-lookup"><span data-stu-id="6e1da-112">Select an existing general ledger account.</span></span> <span data-ttu-id="6e1da-113">En la pestaña **Inicio**, elija **Editar** para abrir la ventana **Ficha cuenta**.</span><span class="sxs-lookup"><span data-stu-id="6e1da-113">On the **Home** tab, choose **Edit** to open the **G/L Account Card** window.</span></span>  
  
3.  <span data-ttu-id="6e1da-114">Amplíe la ficha desplegable **General**.</span><span class="sxs-lookup"><span data-stu-id="6e1da-114">Expand the **General** FastTab.</span></span>  
  
4.  <span data-ttu-id="6e1da-115">En el campo **Cta. regularización**, seleccione la cuenta de ajuste para la cuenta comercial auxiliar.</span><span class="sxs-lookup"><span data-stu-id="6e1da-115">In the **Income Stmt. Bal. Acc.** field, select the adjustment account for the auxiliary commercial account.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="6e1da-116">Dicha cuenta será en la que se cargarán o abonarán los saldos al ejecutar el proceso de regularización.</span><span class="sxs-lookup"><span data-stu-id="6e1da-116">During adjustment, balances will be expensed or credited to this account.</span></span>  
  
5.  <span data-ttu-id="6e1da-117">Escriba la información en los campos requeridos y, a continuación, elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="6e1da-117">Enter information into the required fields, and then choose the **OK** button.</span></span>  
  
### <a name="to-close-income-statement-balances"></a><span data-ttu-id="6e1da-118">Para el asiento de la regularización</span><span class="sxs-lookup"><span data-stu-id="6e1da-118">To close income statement balances</span></span>  
  
1.  <span data-ttu-id="6e1da-119">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cerrar asiento de regularización** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="6e1da-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Close Income Statement**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="6e1da-120">En la ficha desplegable **Opciones**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="6e1da-120">In the **Options** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="6e1da-121">Campo</span><span class="sxs-lookup"><span data-stu-id="6e1da-121">Field</span></span>|<span data-ttu-id="6e1da-122">Description</span><span class="sxs-lookup"><span data-stu-id="6e1da-122">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="6e1da-123">**Fecha final ejercicio**</span><span class="sxs-lookup"><span data-stu-id="6e1da-123">**Fiscal Year Ending Date**</span></span>|<span data-ttu-id="6e1da-124">Seleccione la fecha del ejercicio cerrado.</span><span class="sxs-lookup"><span data-stu-id="6e1da-124">Select the date of the closed fiscal year.</span></span>|  
    |<span data-ttu-id="6e1da-125">**Libro del diario general**</span><span class="sxs-lookup"><span data-stu-id="6e1da-125">**Gen. Journal Template**</span></span>|<span data-ttu-id="6e1da-126">Seleccione el libro del diario general requerido.</span><span class="sxs-lookup"><span data-stu-id="6e1da-126">Select the required general journal template.</span></span>|  
    |<span data-ttu-id="6e1da-127">**Sección diario general**</span><span class="sxs-lookup"><span data-stu-id="6e1da-127">**Gen. Journal Batch**</span></span>|<span data-ttu-id="6e1da-128">Seleccione la sección del diario general requerida.</span><span class="sxs-lookup"><span data-stu-id="6e1da-128">Select the required general journal batch.</span></span>|  
    |<span data-ttu-id="6e1da-129">**Nº documento**</span><span class="sxs-lookup"><span data-stu-id="6e1da-129">**Document No.**</span></span>|<span data-ttu-id="6e1da-130">Escriba el número de documento.</span><span class="sxs-lookup"><span data-stu-id="6e1da-130">Enter the document number.</span></span>|  
    |<span data-ttu-id="6e1da-131">**Cta. ajtes. red. div. adic**</span><span class="sxs-lookup"><span data-stu-id="6e1da-131">**Retained Earnings Acc.**</span></span>|<span data-ttu-id="6e1da-132">Seleccione la cuenta de movimientos de remanente.</span><span class="sxs-lookup"><span data-stu-id="6e1da-132">Select the account for the retained earnings entries.</span></span>|  
    |<span data-ttu-id="6e1da-133">**Texto de registro**</span><span class="sxs-lookup"><span data-stu-id="6e1da-133">**Posting Description**</span></span>|<span data-ttu-id="6e1da-134">Escriba la descripción requerida.</span><span class="sxs-lookup"><span data-stu-id="6e1da-134">Enter the required description.</span></span>|  
  
3.  <span data-ttu-id="6e1da-135">En la sección **Cerrado por**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="6e1da-135">In the **Close by** section, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="6e1da-136">Campo</span><span class="sxs-lookup"><span data-stu-id="6e1da-136">Field</span></span>|<span data-ttu-id="6e1da-137">Description</span><span class="sxs-lookup"><span data-stu-id="6e1da-137">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="6e1da-138">**Código de empresa**</span><span class="sxs-lookup"><span data-stu-id="6e1da-138">**Business Unit Code**</span></span>|<span data-ttu-id="6e1da-139">Seleccione esta opción para crear un movimiento para cada código de empresa.</span><span class="sxs-lookup"><span data-stu-id="6e1da-139">Select to create an entry for each business code.</span></span>|  
    |<span data-ttu-id="6e1da-140">**Dimensiones**</span><span class="sxs-lookup"><span data-stu-id="6e1da-140">**Dimensions**</span></span>|<span data-ttu-id="6e1da-141">Seleccione esta opción para crear un movimiento para cada dimensión de contabilidad.</span><span class="sxs-lookup"><span data-stu-id="6e1da-141">Select to create an entry for each general ledger dimension.</span></span>|  
    |<span data-ttu-id="6e1da-142">**Periodo inventario cerrado**</span><span class="sxs-lookup"><span data-stu-id="6e1da-142">**Inventory Period Closed**</span></span>|<span data-ttu-id="6e1da-143">Seleccione esta opción para indicar que el periodo de inventario con fecha final igual o posterior a la fecha final del periodo contable está cerrado.</span><span class="sxs-lookup"><span data-stu-id="6e1da-143">Select to indicate that the inventory period with ending dates equal to or greater than the last date of the accounting period is closed.</span></span>|  
  
4.  <span data-ttu-id="6e1da-144">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="6e1da-144">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="6e1da-145">Consulte también</span><span class="sxs-lookup"><span data-stu-id="6e1da-145">See Also</span></span>  
 [<span data-ttu-id="6e1da-146">Funcionalidad local para España</span><span class="sxs-lookup"><span data-stu-id="6e1da-146">Spain Local Functionality</span></span>](spain-local-functionality.md)
