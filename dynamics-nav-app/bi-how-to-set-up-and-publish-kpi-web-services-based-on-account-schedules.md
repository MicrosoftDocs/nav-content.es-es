---
title: Configurar y publicar un servicio web KPI que se basa en esquemas de cuentas
description: "En la ventana **Configuración de servicio Web KPI de esquema de cuentas**, se configura cómo mostrar los datos KPI del esquema de cuentas y en qué esquemas de cuentas específicos se deben basar los KPI."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b45fe6e1e5d4e5be00a6e8a34b7b4fea39b5d75b
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules"></a><span data-ttu-id="e3933-103">Procedimiento: configurar y publicar un servicio web KPI que se basa en esquemas de cuentas</span><span class="sxs-lookup"><span data-stu-id="e3933-103">How to: Set Up and Publish KPI Web Services Based on Account Schedules</span></span>
<span data-ttu-id="e3933-104">En la ventana **Configuración de servicio Web KPI de esquema de cuentas**, se configura cómo mostrar los datos KPI del esquema de cuentas y en qué esquemas de cuentas específicos se deben basar los KPI.</span><span class="sxs-lookup"><span data-stu-id="e3933-104">In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.</span></span> <span data-ttu-id="e3933-105">Cuando elige el botón **Publicar servicio Web**, los datos especificados KPI de esquema de cuentas se agregan a la lista de servicios Web publicados en la ventana **Servicios Web**.</span><span class="sxs-lookup"><span data-stu-id="e3933-105">When you choose the **Publish Web Service** button, the specified account-schedule KPI data is added to the list of published web services in the **Web Services** window.</span></span>  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a><span data-ttu-id="e3933-106">Para configurar y publicar un servicio web KPI que se basa en esquemas de cuentas</span><span class="sxs-lookup"><span data-stu-id="e3933-106">To set up and publish a KPI web service that is based on account schedules</span></span>  

1.  <span data-ttu-id="e3933-107">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Configuración del servicio Web KPI de esquema de cuenta** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="e3933-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedule KPI Web Service Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e3933-108">En la ficha desplegable **General**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="e3933-108">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e3933-109">Campo</span><span class="sxs-lookup"><span data-stu-id="e3933-109">Field</span></span>|<span data-ttu-id="e3933-110">Description</span><span class="sxs-lookup"><span data-stu-id="e3933-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e3933-111">**Inicio de valores previstos**</span><span class="sxs-lookup"><span data-stu-id="e3933-111">**Forecasted Values Start**</span></span>|<span data-ttu-id="e3933-112">Especifique en qué momento se muestran los valores previstos en el gráfico KPI del esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-112">Specify at what point in time forecasted values are shown on the account-schedule KPI graphic.</span></span><br /><br /> <span data-ttu-id="e3933-113">Los valores previstos se recuperan del presupuesto de contabilidad general que seleccione en el campo **Nombre presupuesto contable**.</span><span class="sxs-lookup"><span data-stu-id="e3933-113">The forecasted values are retrieved from the general ledger budget that you select in the **G/L Budget Name** field.</span></span> <span data-ttu-id="e3933-114">**Nota**: Para obtener KPI que muestren cifras previstas tras una fecha determinada y cifras reales antes de la fecha, puede cambiar el campo **Permitir registro desde** en la ventana **Configuración de contabilidad**.</span><span class="sxs-lookup"><span data-stu-id="e3933-114">**Note:**  To obtain KPIs that show forecasted figures after a certain date and actual figures before the date, you can change the **Allow Posting From** field in the **General Ledger Setup** window.</span></span> <span data-ttu-id="e3933-115">Para obtener más información, consulte Permitir registrar desde.</span><span class="sxs-lookup"><span data-stu-id="e3933-115">For more information, see Allow Posting From.</span></span>|  
    |<span data-ttu-id="e3933-116">**Nombres pptos. contabilidad<**</span><span class="sxs-lookup"><span data-stu-id="e3933-116">**G/L Budget Name**</span></span>|<span data-ttu-id="e3933-117">Especifique el nombre del presupuesto de contabilidad que proporciona los valores previstos en el servicio web KPI de esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-117">Specify the name of the general ledger budget that provides forecasted values to the account-schedule KPI web service.</span></span>|  
    |<span data-ttu-id="e3933-118">**Periodo**</span><span class="sxs-lookup"><span data-stu-id="e3933-118">**Period**</span></span>|<span data-ttu-id="e3933-119">Especifique el periodo en el que se basa el servicio web KPI de esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-119">Specify the period that the account-schedule KPI web service is based on.</span></span>|  
    |<span data-ttu-id="e3933-120">**Ver por**</span><span class="sxs-lookup"><span data-stu-id="e3933-120">**View By**</span></span>|<span data-ttu-id="e3933-121">Especifiqué en qué intervalo de tiempo se muestra el KPI de esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-121">Specify which time interval the account-schedule KPI is shown in.</span></span>|  
    |<span data-ttu-id="e3933-122">**Nombre del servicio web**</span><span class="sxs-lookup"><span data-stu-id="e3933-122">**Web Service Name**</span></span>|<span data-ttu-id="e3933-123">Especifique el nombre del servicio web KPI de esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-123">Specify the name of the account-schedule KPI web service.</span></span><br /><br /> <span data-ttu-id="e3933-124">Este nombre aparecerá en el campo **Nombre servicio** de la ventana **Servicios web**.</span><span class="sxs-lookup"><span data-stu-id="e3933-124">This name will appear in the **Service Name** field in the **Web Services** window.</span></span>|  

    <span data-ttu-id="e3933-125">Continúe especificando uno o varios esquemas de cuentas que desee publicar como servicio web de KPI según la configuración que ha realizado en la tabla anterior.</span><span class="sxs-lookup"><span data-stu-id="e3933-125">Proceed to specify one or more account schedules that you want to publish as a KPI web service according to the setup that you made in the previous table.</span></span>  

3.  <span data-ttu-id="e3933-126">En la ficha desplegable **Esquemas de cuentas**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="e3933-126">On the **Account Schedules** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e3933-127">Campo</span><span class="sxs-lookup"><span data-stu-id="e3933-127">Field</span></span>|<span data-ttu-id="e3933-128">Description</span><span class="sxs-lookup"><span data-stu-id="e3933-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e3933-129">**Nombre esq. cuentas**</span><span class="sxs-lookup"><span data-stu-id="e3933-129">**Acc. Schedule Name**</span></span>|<span data-ttu-id="e3933-130">Especifique el esquema de cuentas en el que se basa el servicio web KPI.</span><span class="sxs-lookup"><span data-stu-id="e3933-130">Specify the account schedule that the KPI web service is based on.</span></span>|  
    |<span data-ttu-id="e3933-131">**Descripción esq. cuentas**</span><span class="sxs-lookup"><span data-stu-id="e3933-131">**Acc. Schedule Description**</span></span>|<span data-ttu-id="e3933-132">Especifique la descripción del esquema de cuentas en la que se basa el servicio web KPI.</span><span class="sxs-lookup"><span data-stu-id="e3933-132">Specify the description of the account schedule that the KPI web service is based on.</span></span>|  

4.  <span data-ttu-id="e3933-133">Repita el paso 3 para todos los esquemas de cuentas en los que desea basar el servicio web KPI de esquema de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e3933-133">Repeat step 3 for all the account schedules that you want to base the account-schedule KPI web service on.</span></span>  
5.  <span data-ttu-id="e3933-134">Para ver o editar el esquema de cuentas seleccionado, en la ficha desplegable **Esquema de cuentas**, elija **Editar esquema cuentas**.</span><span class="sxs-lookup"><span data-stu-id="e3933-134">To view or edit the selected account schedule, on the **Account Schedule** FastTab, choose the **Edit Account Schedule** action.</span></span>  
6.  <span data-ttu-id="e3933-135">Para ver los datos KPI del esquema de cuentas que ha configurado, elija la acción **Servicio Web KPI de esquema de cuentas**.</span><span class="sxs-lookup"><span data-stu-id="e3933-135">To view the account-schedule KPI data that you have set up, choose the **Account Schedule KPI Web Service** action.</span></span>  
7.  <span data-ttu-id="e3933-136">Para publicar el servicio Web KPI de esquema de cuentas, elija la acción **Publicar servicio Web**.</span><span class="sxs-lookup"><span data-stu-id="e3933-136">To publish the account-schedule KPI web service, choose the **Publish Web Service** action.</span></span> <span data-ttu-id="e3933-137">El servicio web se agrega a la lista de servicios web publicados en la ventana **Servicios web**.</span><span class="sxs-lookup"><span data-stu-id="e3933-137">The web service is added to the list of published web services in the **Web Services** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="e3933-138">También puede publicar el servicio web KPI seleccionando el objeto de la página **Configuración de servicio web KPI de esquema de cuentas** de la ventana **Servicios Web**.</span><span class="sxs-lookup"><span data-stu-id="e3933-138">You can also publish the KPI web service by pointing to the **Account Schedule KPI Web Service Setup** page object from the **Web Services** window.</span></span> <span data-ttu-id="e3933-139">Para obtener más información, consulte [Cómo publicar un servicio Web](https://msdn.microsoft.com/en-us/library/dd338978.aspx) en MSDN.</span><span class="sxs-lookup"><span data-stu-id="e3933-139">For more information, see [How to: Publish a Web Service](https://msdn.microsoft.com/en-us/library/dd338978.aspx) on MSDN.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e3933-140">Consulte también</span><span class="sxs-lookup"><span data-stu-id="e3933-140">See Also</span></span>  
[<span data-ttu-id="e3933-141">Inteligencia empresarial</span><span class="sxs-lookup"><span data-stu-id="e3933-141">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="e3933-142">Finanzas</span><span class="sxs-lookup"><span data-stu-id="e3933-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="e3933-143">Configurar las finanzas</span><span class="sxs-lookup"><span data-stu-id="e3933-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="e3933-144">Libro mayor y plan de cuentas</span><span class="sxs-lookup"><span data-stu-id="e3933-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="e3933-145">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e3933-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
