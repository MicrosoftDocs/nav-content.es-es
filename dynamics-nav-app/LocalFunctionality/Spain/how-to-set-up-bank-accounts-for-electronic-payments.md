---
title: "Configurar cuentas bancarias para realizar pagos electrónicos"
description: "En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede configurar cuentas bancarias para realizar pagos electrónicos."
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
ms.openlocfilehash: 618873f866bd48774e70d7df56f023cbc13ca84a
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-accounts-for-electronic-payments"></a><span data-ttu-id="cf822-103">Configurar cuentas bancarias para realizar pagos electrónicos</span><span class="sxs-lookup"><span data-stu-id="cf822-103">How to: Set Up Bank Accounts for Electronic Payments</span></span>
<span data-ttu-id="cf822-104">En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede configurar cuentas bancarias para realizar pagos electrónicos.</span><span class="sxs-lookup"><span data-stu-id="cf822-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can set up bank accounts to make electronic payments.</span></span>  
  
### <a name="to-set-up-bank-accounts-for-electronic-payments"></a><span data-ttu-id="cf822-105">Para configurar cuentas bancarias para realizar pagos electrónicos</span><span class="sxs-lookup"><span data-stu-id="cf822-105">To set up bank accounts for electronic payments</span></span>  
  
1.  <span data-ttu-id="cf822-106">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ficha banco** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="cf822-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Account Card**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="cf822-107">En la ficha desplegable **Transferencia**, asegúrese de que los campos **CCC Cód. banco**, **CCC Cód. oficina**, **CCC Dígito control** y **CCC Nº cuenta** se rellenan correctamente.</span><span class="sxs-lookup"><span data-stu-id="cf822-107">On the **Transfer** FastTab, make sure that the **CCC Bank No.**, **CCC Bank Branch No.**, **CCC Control Digits**, and **CCC Bank Account No.** fields are filled in correctly.</span></span>  
  
3.  <span data-ttu-id="cf822-108">En la ficha desplegable **Transferencia**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="cf822-108">On the **Transfer** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="cf822-109">Campo</span><span class="sxs-lookup"><span data-stu-id="cf822-109">Field</span></span>|<span data-ttu-id="cf822-110">Description</span><span class="sxs-lookup"><span data-stu-id="cf822-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cf822-111">**Ruta archivo exp. pago elec.**</span><span class="sxs-lookup"><span data-stu-id="cf822-111">**E-Pay Export File Path**</span></span>|<span data-ttu-id="cf822-112">Introduzca la ruta de acceso completa del archivo de pago electrónico, empiece con la letra de la unidad y acabe con una barra diagonal inversa (\).</span><span class="sxs-lookup"><span data-stu-id="cf822-112">Enter the full path of the electronic payment file, start with the drive letter and end with a backslash ().</span></span> <span data-ttu-id="cf822-113">El nombre no se escribe aquí.</span><span class="sxs-lookup"><span data-stu-id="cf822-113">The file name is not included here.</span></span> <span data-ttu-id="cf822-114">Debe utilizar el directorio donde [!INCLUDE[navnow](../../includes/navnow_md.md)] se encuentra instalado.</span><span class="sxs-lookup"><span data-stu-id="cf822-114">You should use the directory where [!INCLUDE[navnow](../../includes/navnow_md.md)] is installed.</span></span> <span data-ttu-id="cf822-115">Por ejemplo, podría escribir **C:NAV** en este campo.</span><span class="sxs-lookup"><span data-stu-id="cf822-115">For example: **C:NAV** would be a possible entry for this field.</span></span> <span data-ttu-id="cf822-116">Puede escribir 100 caracteres como máximo.</span><span class="sxs-lookup"><span data-stu-id="cf822-116">You can enter a maximum of 100 characters.</span></span>|  
    |<span data-ttu-id="cf822-117">**Nom. arch. exp. últ. pago elec.**</span><span class="sxs-lookup"><span data-stu-id="cf822-117">**Last E-Pay Export File Name**</span></span>|<span data-ttu-id="cf822-118">Especifique el nombre del archivo con la extensión de nombre de archivo .txt, sin la ruta. Debido a que el nombre del archivo se incrementará cada vez que se exporte un archivo de pago electrónico, este nombre de archivo debe tener dígitos.</span><span class="sxs-lookup"><span data-stu-id="cf822-118">Specify the name of the file with the .txt file name extension, without the path., Because the file name will be incremented every time that an electronic payment file is exported, this file name should have digits in it.</span></span> <span data-ttu-id="cf822-119">De esta forma se creará un registro permanente de cada archivo que haya exportado al banco.</span><span class="sxs-lookup"><span data-stu-id="cf822-119">This will create a permanent record of every file that you have exported to the bank.</span></span> <span data-ttu-id="cf822-120">Por ejemplo, **DD000000.txt** podría ser la primera entrada de este campo.</span><span class="sxs-lookup"><span data-stu-id="cf822-120">For example, **DD000000.txt** could be a possible first entry for this field.</span></span> <span data-ttu-id="cf822-121">Puede escribir 50 caracteres como máximo.</span><span class="sxs-lookup"><span data-stu-id="cf822-121">You can enter a maximum of 50 characters.</span></span>|  
  
4.  <span data-ttu-id="cf822-122">En la ficha desplegable **Registrando**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="cf822-122">On the **Posting** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="cf822-123">Campo</span><span class="sxs-lookup"><span data-stu-id="cf822-123">Field</span></span>|<span data-ttu-id="cf822-124">Description</span><span class="sxs-lookup"><span data-stu-id="cf822-124">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cf822-125">**Nº último aviso pago**</span><span class="sxs-lookup"><span data-stu-id="cf822-125">**Last Remittance Advice No.**</span></span>|<span data-ttu-id="cf822-126">Especifique una serie de números distinta a la serie de números de los cheques.</span><span class="sxs-lookup"><span data-stu-id="cf822-126">Specify a number series that differs from the check number series.</span></span> <span data-ttu-id="cf822-127">Esto es necesario para que los números no entren en conflicto entre sí.</span><span class="sxs-lookup"><span data-stu-id="cf822-127">This is needed so that the numbers do not conflict with each other.</span></span> <span data-ttu-id="cf822-128">El aviso de pago se imprime en papel en blanco de forma que resulte fácil enviarlo al proveedor.</span><span class="sxs-lookup"><span data-stu-id="cf822-128">The remittance advice is printed on blank paper in a form that is easy to mail to the vendor.</span></span>|  
  
### <a name="to-set-up-vendor-bank-accounts-for-electronic-payments"></a><span data-ttu-id="cf822-129">Para configurar cuentas bancarias para realizar pagos electrónicos</span><span class="sxs-lookup"><span data-stu-id="cf822-129">To set up vendor bank accounts for electronic payments</span></span>  
  
1.  <span data-ttu-id="cf822-130">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ficha banco proveedor** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="cf822-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Bank Account Card**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="cf822-131">En la ficha desplegable **General**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="cf822-131">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="cf822-132">Campo</span><span class="sxs-lookup"><span data-stu-id="cf822-132">Field</span></span>|<span data-ttu-id="cf822-133">Description</span><span class="sxs-lookup"><span data-stu-id="cf822-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cf822-134">**Usar para pagos electrónicos**</span><span class="sxs-lookup"><span data-stu-id="cf822-134">**Use For Electronic Payments**</span></span>|<span data-ttu-id="cf822-135">Especifica si debe usarse esta cuenta bancaria del proveedor para los pagos electrónicos.</span><span class="sxs-lookup"><span data-stu-id="cf822-135">Specify if this vendor bank account will be used for electronic payments.</span></span> <span data-ttu-id="cf822-136">Para realizar pagos electrónicos solo se puede seleccionar una cuenta de banco por proveedor.</span><span class="sxs-lookup"><span data-stu-id="cf822-136">For electronic payments, only one bank account can be selected for each vendor.</span></span>|  
  
3.  <span data-ttu-id="cf822-137">En la ficha desplegable **Transferencia**, asegúrese de que los campos **CCC Cód. banco**, **CCC Cód. oficina**, **CCC Dígito control** y **CCC Nº cuenta** se rellenan correctamente.</span><span class="sxs-lookup"><span data-stu-id="cf822-137">On the **Transfer** FastTab, make sure that the **CCC Bank No.**, **CCC Bank Branch No.**, **CCC Control Digits**, and **CCC Bank Account No.** fields are filled in correctly.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="cf822-138">Consulte también</span><span class="sxs-lookup"><span data-stu-id="cf822-138">See Also</span></span>  
 [<span data-ttu-id="cf822-139">Pagos electrónicos – AEB N34.1</span><span class="sxs-lookup"><span data-stu-id="cf822-139">Electronic Payments – AEB N34.1</span></span>](electronic-payments-%E2%80%93-aeb-n34.1.md)