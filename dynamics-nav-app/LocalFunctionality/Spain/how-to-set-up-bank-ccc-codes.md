---
title: "Configuración de códigos CCC de bancos"
description: "El Código Cuenta Cliente (CCC) es un código de cuenta único usado por los bancos para identificar a sus clientes. El código CCC se imprime en los documentos bancarios, como cheques y extractos."
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
ms.openlocfilehash: 7169b7f3bb51b51000c9187d3b9887bf89118f84
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-ccc-codes"></a><span data-ttu-id="37f1f-104">Configuración de códigos CCC de bancos</span><span class="sxs-lookup"><span data-stu-id="37f1f-104">How to: Set Up Bank CCC Codes</span></span>
<span data-ttu-id="37f1f-105">El Código Cuenta Cliente (CCC) es un código de cuenta único usado por los bancos para identificar a sus clientes.</span><span class="sxs-lookup"><span data-stu-id="37f1f-105">Código Cuenta Cliente (CCC) is a unique account code used by banks to identify their customers.</span></span> <span data-ttu-id="37f1f-106">El código CCC se imprime en los documentos bancarios, como cheques y extractos.</span><span class="sxs-lookup"><span data-stu-id="37f1f-106">The CCC code is printed on bank documents such as checks and statements.</span></span>  
  
 <span data-ttu-id="37f1f-107">Se pueden configurar códigos CCC en las siguientes ubicaciones:</span><span class="sxs-lookup"><span data-stu-id="37f1f-107">You can set up CCC codes in the following locations:</span></span>  
  
-   <span data-ttu-id="37f1f-108">Ventana **Ficha banco**</span><span class="sxs-lookup"><span data-stu-id="37f1f-108">**Bank Account Card** window</span></span>  
  
-   <span data-ttu-id="37f1f-109">Ventana **Información empresa**</span><span class="sxs-lookup"><span data-stu-id="37f1f-109">**Company Information** window</span></span>  
  
-   <span data-ttu-id="37f1f-110">Ventana **Ficha banco cliente**</span><span class="sxs-lookup"><span data-stu-id="37f1f-110">**Customer Bank Account Card** window</span></span>  
  
-   <span data-ttu-id="37f1f-111">Ventana **Ficha banco proveedor**</span><span class="sxs-lookup"><span data-stu-id="37f1f-111">**Vendor Bank Account Card** window</span></span>  
  
 <span data-ttu-id="37f1f-112">El procedimiento siguiente describe cómo configurar códigos CCC de banco para su empresa.</span><span class="sxs-lookup"><span data-stu-id="37f1f-112">The following procedure describes how to set up bank CCC codes for your company.</span></span>  
  
### <a name="to-enter-ccc-codes"></a><span data-ttu-id="37f1f-113">Para introducir códigos CCC</span><span class="sxs-lookup"><span data-stu-id="37f1f-113">To enter CCC codes</span></span>  
  
1.  <span data-ttu-id="37f1f-114">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Información de la empresa** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="37f1f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="37f1f-115">Rellene los campos de la ficha desplegable **Pagos**, tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="37f1f-115">On the **Payments** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="37f1f-116">Campo</span><span class="sxs-lookup"><span data-stu-id="37f1f-116">Field</span></span>|<span data-ttu-id="37f1f-117">Description</span><span class="sxs-lookup"><span data-stu-id="37f1f-117">Description</span></span>|  
    |---------------------------------|--------------|---------------------------------------|  
    |<span data-ttu-id="37f1f-118">**CCC Cód. banco**</span><span class="sxs-lookup"><span data-stu-id="37f1f-118">**CCC Bank No.**</span></span>|<span data-ttu-id="37f1f-119">1-4</span><span class="sxs-lookup"><span data-stu-id="37f1f-119">1-4</span></span>|<span data-ttu-id="37f1f-120">Identifica el banco en el que se ha abierto la cuenta.</span><span class="sxs-lookup"><span data-stu-id="37f1f-120">Identifies the bank where the account has been opened.</span></span>|  
    |<span data-ttu-id="37f1f-121">**CCC Cód. oficina**</span><span class="sxs-lookup"><span data-stu-id="37f1f-121">**CCC Bank Branch No.**</span></span>|<span data-ttu-id="37f1f-122">5-8</span><span class="sxs-lookup"><span data-stu-id="37f1f-122">5-8</span></span>|<span data-ttu-id="37f1f-123">Identifica el código de la oficina.</span><span class="sxs-lookup"><span data-stu-id="37f1f-123">Identifies the branch code.</span></span> <span data-ttu-id="37f1f-124">Si el banco no utiliza esta referencia, el código de la oficina pueden ser ceros.</span><span class="sxs-lookup"><span data-stu-id="37f1f-124">If the bank does not use this reference, the branch code can be zeros.</span></span>|  
    |<span data-ttu-id="37f1f-125">**CCC Dígito control**</span><span class="sxs-lookup"><span data-stu-id="37f1f-125">**CCC Control Digits**</span></span>|<span data-ttu-id="37f1f-126">9-10</span><span class="sxs-lookup"><span data-stu-id="37f1f-126">9-10</span></span>|<span data-ttu-id="37f1f-127">Identifica los dígitos de control.</span><span class="sxs-lookup"><span data-stu-id="37f1f-127">Identifies the control digits.</span></span>|  
    |<span data-ttu-id="37f1f-128">**CCC Nº cuenta**</span><span class="sxs-lookup"><span data-stu-id="37f1f-128">**CCC Bank Account No.**</span></span>|<span data-ttu-id="37f1f-129">11-20 (España)</span><span class="sxs-lookup"><span data-stu-id="37f1f-129">11-20 (Spain)</span></span><br /><br /> <span data-ttu-id="37f1f-130">11-21 (Portugal)</span><span class="sxs-lookup"><span data-stu-id="37f1f-130">11-21 (Portugal)</span></span>|<span data-ttu-id="37f1f-131">Identifica el número de cuenta, que se puede ajustar con ceros a la izquierda.</span><span class="sxs-lookup"><span data-stu-id="37f1f-131">Identifies the account number, which may be adjusted with preceding zeros.</span></span>|  
  
 <span data-ttu-id="37f1f-132">El siguiente procedimiento describe cómo configurar códigos bancarios CCC para cuentas bancarias de clientes existentes, pero los mismos pasos se aplican a proveedores, cuentas bancarias e información de la compañía.</span><span class="sxs-lookup"><span data-stu-id="37f1f-132">The following procedure describes how to set up bank CCC codes for existing customer bank accounts, but the same steps apply to vendors, bank accounts, and company information.</span></span>  
  
### <a name="to-set-up-bank-ccc-codes-for-a-customer-bank-account"></a><span data-ttu-id="37f1f-133">Para configurar códigos CCC de banco de un banco cliente</span><span class="sxs-lookup"><span data-stu-id="37f1f-133">To set up bank CCC codes for a customer bank account</span></span>  
  
1.  <span data-ttu-id="37f1f-134">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ficha banco cliente** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="37f1f-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Bank Account Card**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="37f1f-135">En la ficha desplegable **Transferencia**, escriba la información en los campos CCC relevantes.</span><span class="sxs-lookup"><span data-stu-id="37f1f-135">On the **Transfer** FastTab, enter information into the relevant CCC fields.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="37f1f-136">Debe configurar información de la empresa en la ficha desplegable **Pagos**.</span><span class="sxs-lookup"><span data-stu-id="37f1f-136">You must set up the company information on the **Payments** FastTab.</span></span>  
  
3.  <span data-ttu-id="37f1f-137">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="37f1f-137">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="37f1f-138">Consulte también</span><span class="sxs-lookup"><span data-stu-id="37f1f-138">See Also</span></span>  
 <span data-ttu-id="37f1f-139">[Procedimiento para introducir la información de la empresa](how-to-enter-company-information.md) </span><span class="sxs-lookup"><span data-stu-id="37f1f-139">[How to: Enter Company Information](how-to-enter-company-information.md) </span></span>  
 <span data-ttu-id="37f1f-140">[Procedimiento para configurar las cuentas de bancos](how-to-set-up-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="37f1f-140">[How to: Set Up Bank Accounts](how-to-set-up-bank-accounts.md) </span></span>  
 <span data-ttu-id="37f1f-141">Ficha banco cliente</span><span class="sxs-lookup"><span data-stu-id="37f1f-141">Customer Bank Account Card</span></span>   
 [<span data-ttu-id="37f1f-142">Configuración de bancos de proveedores</span><span class="sxs-lookup"><span data-stu-id="37f1f-142">How to: Set Up Vendor Bank Accounts</span></span>](how-to-set-up-vendor-bank-accounts.md)