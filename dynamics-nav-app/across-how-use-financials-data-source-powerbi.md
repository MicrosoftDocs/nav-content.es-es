---
title: Crear un origen de datos de Power BI con Dynamics NAV
description: "Puede hacer que los datos de Dynamics NAV estén disponibles como origen de datos en Power BI y generar informes eficaces del estado de la empresa."
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b1beb7286eb221e5df3e7d5b2050ddcb389a0a07
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="using-included365finincludesd365finmdmd-as-a-power-bi-data-source"></a><span data-ttu-id="6ad0b-103">Usar [!INCLUDE[d365fin](includes/d365fin_md.md)] como origen de datos de Power BI</span><span class="sxs-lookup"><span data-stu-id="6ad0b-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source</span></span>
<span data-ttu-id="6ad0b-104">Puede hacer que los datos de [!INCLUDE[d365fin](includes/d365fin_md.md)] estén disponibles como origen de datos en Power BI y generar informes eficaces del estado de la empresa.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="6ad0b-105">Debe disponer de una cuenta válida con [!INCLUDE[d365fin](includes/d365fin_md.md)] y con Power BI.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="6ad0b-106">Además, deberá descargar [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="6ad0b-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="6ad0b-107">Para agregar [!INCLUDE[d365fin](includes/d365fin_md.md)] como origen de datos de Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="6ad0b-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span></span>
1. <span data-ttu-id="6ad0b-108">En Power BI Desktop, en el panel de navegador izquierdo, elija **Obtener datos**.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="6ad0b-109">En la ventana **Obtener datos**, **Servicios en línea**, elija **Dynamics NAV** y después seleccione el botón **Conectar**.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics NAV**, and then choose the **Connect** button.</span></span>

   <span data-ttu-id="6ad0b-110">Power BI muestra un asistente que le guiará por el proceso de conexión.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-110">Power BI displays a wizard that will guide you though the connection process.</span></span> <span data-ttu-id="6ad0b-111">El primer paso será especificar una dirección URL de OData y el nombre de la empresa que está asociada a la cuenta de [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6ad0b-111">The first step will be to enter an OData URL and the company name that is associated with your [!INCLUDE[d365fin](includes/d365fin_md.md)] account.</span></span>  

   <span data-ttu-id="6ad0b-112">Para *URL de OData*, puede copiar la dirección URL de OData V4 de cualquiera de los servicios web que se muestran en la página **Servicios Web** en [!INCLUDE[d365fin](includes/d365fin_md.md)], por ejemplo, `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-112">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span></span>  

   <span data-ttu-id="6ad0b-113">Para *Nombre empresa*, utilice el nombre que se muestra en el campo **Nombre** de la ventana **Información empresa** en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6ad0b-113">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6ad0b-114">Si [!INCLUDE[d365fin](includes/d365fin_md.md)] contiene varias empresas, elija el nombre de la empresa pertinente en la lista en la ventana **Empresas**.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-114">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span></span> <span data-ttu-id="6ad0b-115">En ambos casos, asegúrese de que el nombre que especifique en el asistente Power BI coincide exactamente con el texto que se muestra en [!INCLUDE[d365fin](includes/d365fin_md.md)], como `My Company`.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-115">In both cases, make sure that the name that you specify in the Power BI wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span></span>
3. <span data-ttu-id="6ad0b-116">Una vez introducidos los datos, elija el botón Aceptar.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-116">Once you have entered the information, choose the OK button.</span></span> <span data-ttu-id="6ad0b-117">El siguiente paso en el asistente es introducir su nombre de usuario y contraseña.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-117">The next step in the wizard will be to enter your username and password.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="6ad0b-118">Si hay otras opciones de autenticación disponibles en el panel de navegación izquierdo, elija *Básico*.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-118">If there are other authentication options available in the left hand navigation, choose *Basic*.</span></span>
4. <span data-ttu-id="6ad0b-119">Introduzca su nombre de usuario y contraseña.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-119">Enter your username and password.</span></span> <span data-ttu-id="6ad0b-120">Puede encontrar esta información en la ventana **Usuarios** en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6ad0b-120">You can find this information in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6ad0b-121">Utilice la **Clave de acceso web** como la contraseña.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-121">Use the **Web Access Key** as your password.</span></span>

   <span data-ttu-id="6ad0b-122">Por ejemplo, su nombre de usuario es *ADMIN* y la clave de acceso al servicio Web que actúa de contraseña es *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span></span>
5. <span data-ttu-id="6ad0b-123">Elija el botón **Conexión** para continuar.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-123">Choose the **Connection** button to continue.</span></span> <span data-ttu-id="6ad0b-124">El asistente Power BI muestra una lista de los orígenes de datos de [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6ad0b-124">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] data sources.</span></span> <span data-ttu-id="6ad0b-125">Este origen de datos todos los servicios web que haya publicado desde [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6ad0b-125">These data source represent all the web services that you have published from your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="6ad0b-126">Si lo desea, puede crear una nueva dirección URL de servicio Web en [!INCLUDE[d365fin](includes/d365fin_md.md)] mediante la acción **Crear conjunto de datos** en la página **Servicios web**, utilizando la guía de configuración asistida **Configurar informes** o eligiendo la acción **Editar en Excel** en cualquier lista.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>

6. <span data-ttu-id="6ad0b-127">Especifique los datos que desea agregar al modelo de datos y después seleccione el botón **Cargar**.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-127">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="6ad0b-128">Repita los pasos anteriores agregar datos de [!INCLUDE[d365fin](includes/d365fin_md.md)] adicionales a su modelo de datos de Power BI.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-128">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="6ad0b-129">Una vez que haya conectado correctamente con [!INCLUDE[d365fin](includes/d365fin_md.md)], no se le solicitará nuevamente la URL, el nombre de usuario o la contraseña de OData.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-129">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span></span>

<span data-ttu-id="6ad0b-130">Una vez que los datos se hayan cargado, aparecerán en el panel de navegación derecho en la página.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-130">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="6ad0b-131">Ya se ha conectado correctamente con los datos de Dynamics NAV y está preparado para comenzar a crear su informe de Power BI.</span><span class="sxs-lookup"><span data-stu-id="6ad0b-131">At this point, you have successfully connected to your Dynamics NAV data and are ready to begin building your Power BI report.</span></span> <span data-ttu-id="6ad0b-132">Para obtener más información, consulte la [documentación de Power BI](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span><span class="sxs-lookup"><span data-stu-id="6ad0b-132">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span></span>

## <a name="see-also"></a><span data-ttu-id="6ad0b-133">Consulte también</span><span class="sxs-lookup"><span data-stu-id="6ad0b-133">See Also</span></span>
[<span data-ttu-id="6ad0b-134">Inteligencia empresarial</span><span class="sxs-lookup"><span data-stu-id="6ad0b-134">Business Intelligence</span></span>](bi.md)  
<span data-ttu-id="6ad0b-135">[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="6ad0b-135">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="6ad0b-136">Importar datos de empresa de otros sistemas financieros</span><span class="sxs-lookup"><span data-stu-id="6ad0b-136">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="6ad0b-137">[Configurar [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="6ad0b-137">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="6ad0b-138">Finanzas</span><span class="sxs-lookup"><span data-stu-id="6ad0b-138">Finance</span></span>](finance.md)  
