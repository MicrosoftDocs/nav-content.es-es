---
title: "Cómo configurar un plan de tipos de coste"
description: El plan de tipos de coste es similar al plan de cuentas de contabilidad general.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger, accounts
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 104b057639090bd9797f06ebcc6b573899b9f87c
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-cost-types"></a><span data-ttu-id="fe33c-103">Procedimiento para configurar centros de costes</span><span class="sxs-lookup"><span data-stu-id="fe33c-103">How to: Set Up Cost Types</span></span>
<span data-ttu-id="fe33c-104">El plan de tipos de coste es similar al plan de cuentas de contabilidad general.</span><span class="sxs-lookup"><span data-stu-id="fe33c-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span></span> <span data-ttu-id="fe33c-105">Puede configurar el plan de tipos de coste de la siguiente forma:</span><span class="sxs-lookup"><span data-stu-id="fe33c-105">You can set up the chart of cost types in the following ways:</span></span>  

-   <span data-ttu-id="fe33c-106">Estructure el plan de tipos de coste de manera similar a las cuentas de ingresos del plan de cuentas de contabilidad general.</span><span class="sxs-lookup"><span data-stu-id="fe33c-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span></span> <span data-ttu-id="fe33c-107">Luego puede transferir el plan de cuentas de contabilidad al plan de tipos de coste.</span><span class="sxs-lookup"><span data-stu-id="fe33c-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span></span> <span data-ttu-id="fe33c-108">Puede hacer los ajustes necesarios después de la transferencia.</span><span class="sxs-lookup"><span data-stu-id="fe33c-108">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="fe33c-109">Cree el nuevo plan de tipos de coste o agregue nuevos tipos de coste al plan existente de tipos de coste.</span><span class="sxs-lookup"><span data-stu-id="fe33c-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span></span> <span data-ttu-id="fe33c-110">Debe crear cada tipo de coste nuevo por separado.</span><span class="sxs-lookup"><span data-stu-id="fe33c-110">You must create each new cost type individually.</span></span>  

## <a name="to-transfer-the-general-ledger-chart-of-accounts-to-the-chart-of-cost-types"></a><span data-ttu-id="fe33c-111">Para transferir el plan de cuentas de contabilidad al plan de tipos de coste</span><span class="sxs-lookup"><span data-stu-id="fe33c-111">To transfer the general ledger chart of accounts to the chart of cost types</span></span>  
1.  <span data-ttu-id="fe33c-112">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan tipos coste** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="fe33c-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fe33c-113">Elija la acción **Traer tipos coste de plan cuentas**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-113">Choose the **Get Cost Types from Chart of Accounts** action.</span></span> <span data-ttu-id="fe33c-114">En el cuadro de diálogo, seleccione el botón **Sí** para confirmar la transferencia.</span><span class="sxs-lookup"><span data-stu-id="fe33c-114">In the dialog box, choose the **Yes** button to confirm the transfer.</span></span> <span data-ttu-id="fe33c-115">La función utiliza el plan de cuentas para crear un plan de tipos de coste.</span><span class="sxs-lookup"><span data-stu-id="fe33c-115">The function uses the chart of accounts to create a chart of cost types.</span></span>  

    <span data-ttu-id="fe33c-116">El plan de tipos de coste contendrá todas las cuentas de ingresos en la contabilidad e incluye títulos y subtotales.</span><span class="sxs-lookup"><span data-stu-id="fe33c-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span></span> <span data-ttu-id="fe33c-117">Puede cambiar el plan de tipos de coste, según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="fe33c-117">You can change the chart of cost types, as necessary.</span></span> <span data-ttu-id="fe33c-118">Por ejemplo, puede eliminar los tipos de coste existentes duplicados.</span><span class="sxs-lookup"><span data-stu-id="fe33c-118">For example, you can delete duplicate existing cost types.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="fe33c-119">La función **Registrar tipos de coste en plan ctas.** actualiza la relación entre el plan de cuentas y el plan de tipos de coste.</span><span class="sxs-lookup"><span data-stu-id="fe33c-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span></span> <span data-ttu-id="fe33c-120">El campo **Nº**</span><span class="sxs-lookup"><span data-stu-id="fe33c-120">The **No.**</span></span> <span data-ttu-id="fe33c-121">se rellena y comprueba para asegurarse de que cada cuenta contable está relacionada con un solo tipo de coste.</span><span class="sxs-lookup"><span data-stu-id="fe33c-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span></span> <span data-ttu-id="fe33c-122">La función se ejecuta automáticamente antes de transferir los movimientos de contabilidad a la contabilidad de costes.</span><span class="sxs-lookup"><span data-stu-id="fe33c-122">The function runs automatically before transferring general ledger entries to cost accounting.</span></span>  

## <a name="to-set-up-new-cost-types-in-the-chart-of-cost-types-window"></a><span data-ttu-id="fe33c-123">Configurar nuevos tipos de coste en la ventana Tipos centros coste</span><span class="sxs-lookup"><span data-stu-id="fe33c-123">To set up new cost types in the Chart of Cost Types window</span></span>  
1.  <span data-ttu-id="fe33c-124">Abra la ventana **Tipos centros coste** en el modo de edición.</span><span class="sxs-lookup"><span data-stu-id="fe33c-124">Open the **Chart of Cost Types** window in edit mode.</span></span>  
2.  <span data-ttu-id="fe33c-125">Rellene los campos descritos como necesarios.</span><span class="sxs-lookup"><span data-stu-id="fe33c-125">Fill in the fields as described as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >  <span data-ttu-id="fe33c-126">Puede configurar y mantener tipos de coste en la ventana **Ficha tipo de coste** o bien en la ventana **Plan tipos coste**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-126">You can set up and maintain cost types in either the **Cost Type Card** window or in the **Chart of Cost Types** window.</span></span> <span data-ttu-id="fe33c-127">En este procedimiento, va a configurar tipos de coste en la ventana **Plan de tipos de coste**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-127">In this procedure, you set up cost types in the **Chart of Cost Types** window.</span></span>

3.  <span data-ttu-id="fe33c-128">Una vez creados todos los tipos de coste, elija la acción **Aplicar sangría a tipos coste**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-128">After you have created all cost types, choose the **Indent Cost Types** action.</span></span> <span data-ttu-id="fe33c-129">En el cuadro de diálogo, elija el botón **Sí**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-129">In the dialog box, choose the **Yes** button.</span></span>  
4.  <span data-ttu-id="fe33c-130">Vincule el nuevo tipo de coste a la cuenta de contabilidad correspondiente.</span><span class="sxs-lookup"><span data-stu-id="fe33c-130">Link the new cost type to the corresponding general ledger account.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="fe33c-131">Si se han escrito definiciones en el campo **Totales** para las cuentas de tipo **Fin-Total** antes de ejecutar la función **Aplicar sangría a tipos coste**, deberá volver a escribir las definiciones más adelante porque la función sobrescribe los valores de todos los campos **Fin-Total**.</span><span class="sxs-lookup"><span data-stu-id="fe33c-131">If you have entered definitions in the **Totaling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="to-update-cost-types"></a><span data-ttu-id="fe33c-132">Para actualizar tipos de coste</span><span class="sxs-lookup"><span data-stu-id="fe33c-132">To update cost types</span></span>  
1.  <span data-ttu-id="fe33c-133">En la ventana **Configuración contabilidad costes**, seleccione si desea que el plan de tipos de coste se actualice automáticamente cuando el plan de cuentas se cambia.</span><span class="sxs-lookup"><span data-stu-id="fe33c-133">In the **Cost Accounting Setup** window, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span></span>  
2.  <span data-ttu-id="fe33c-134">En el campo **Alinear cuenta C/G** puede seleccionar de entre las siguientes opciones.</span><span class="sxs-lookup"><span data-stu-id="fe33c-134">In the **Align G/L Account** field, you can choose from the following options.</span></span>  

- <span data-ttu-id="fe33c-135">**Sin alineación**: no hay cambio aplicable en el plan de tipos de coste cuando se modifica el plan de cuentas.</span><span class="sxs-lookup"><span data-stu-id="fe33c-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="fe33c-136">**Automático**: se realiza el cambio correspondiente en el plan de tipos de coste cuando se modifica el plan de cuentas.</span><span class="sxs-lookup"><span data-stu-id="fe33c-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="fe33c-137">**Solicitud**: se muestra un mensaje que pregunta si desea realizar a cambio correspondiente en el plan de tipos de coste cuando se realiza un cambio en el plan de cuentas.</span><span class="sxs-lookup"><span data-stu-id="fe33c-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fe33c-138">Consulte también</span><span class="sxs-lookup"><span data-stu-id="fe33c-138">See Also</span></span>  
[<span data-ttu-id="fe33c-139">Contabilidad para costes</span><span class="sxs-lookup"><span data-stu-id="fe33c-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="fe33c-140">[Definición de la relación entre los tipos de coste y las cuentas de contabilidad](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="fe33c-140">[Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md) </span></span>  
<span data-ttu-id="fe33c-141">[Definición de centros de coste y de objetos de coste para el plan de cuentas](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="fe33c-141">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span></span>  
<span data-ttu-id="fe33c-142">[Saldos entre el tipo de coste, centro de coste y objeto de coste](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span><span class="sxs-lookup"><span data-stu-id="fe33c-142">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span></span>  
<span data-ttu-id="fe33c-143">[Configuración de contabilidad de costes](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="fe33c-143">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="fe33c-144">[Terminología en contabilidad de costes](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="fe33c-144">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="fe33c-145">Acerca de la contabilidad de costes</span><span class="sxs-lookup"><span data-stu-id="fe33c-145">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="fe33c-146">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fe33c-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
