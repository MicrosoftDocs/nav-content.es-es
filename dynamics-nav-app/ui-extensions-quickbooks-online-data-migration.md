---
title: "Uso de la extensión de la migración de QuickBooks"
description: "Describe cómo utilizar la extensión para migrar clientes, proveedores, elementos y cuentas de QuickBooks Online a Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ff8f8f0c529966fc108d2d4c86e2d0681b1fc005
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="e21fc-103">Extensión de la migración de datos de QuickBooks Online para Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="e21fc-103">The QuickBooks Online Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="e21fc-104">Esta extensión se incluye en la guía de configuración asistida **Migración de datos** para ayudarle a migrar datos comerciales importantes de QuickBooks Online a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e21fc-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e21fc-105">Por ejemplo, esto es útil cuando su negocio está creciendo y ha decidido actualizar su aplicación de administración de negocios con [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e21fc-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="e21fc-106">¿Qué datos puedo importar desde QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="e21fc-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="e21fc-107">Desde QuickBooks Online puede importar a [!INCLUDE[d365fin](includes/d365fin_md.md)] los datos siguientes:</span><span class="sxs-lookup"><span data-stu-id="e21fc-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="e21fc-108">Clientes</span><span class="sxs-lookup"><span data-stu-id="e21fc-108">Customers</span></span>
* <span data-ttu-id="e21fc-109">Proveedores</span><span class="sxs-lookup"><span data-stu-id="e21fc-109">Vendors</span></span>
* <span data-ttu-id="e21fc-110">Productos</span><span class="sxs-lookup"><span data-stu-id="e21fc-110">Items</span></span>
* <span data-ttu-id="e21fc-111">Plan de cuentas</span><span class="sxs-lookup"><span data-stu-id="e21fc-111">Chart of accounts</span></span> 
* <span data-ttu-id="e21fc-112">Comienzo de la transacción de saldo en el libro mayor</span><span class="sxs-lookup"><span data-stu-id="e21fc-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="e21fc-113">Cantidad disponible de productos de inventario</span><span class="sxs-lookup"><span data-stu-id="e21fc-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="e21fc-114">Documentos pendientes para clientes y proveedores, como facturas, abonos y pagos</span><span class="sxs-lookup"><span data-stu-id="e21fc-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="e21fc-115">Migramos únicamente los importes totales de los documentos de ventas y compras.</span><span class="sxs-lookup"><span data-stu-id="e21fc-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="e21fc-116">No actualizamos importes pagados parcialmente.</span><span class="sxs-lookup"><span data-stu-id="e21fc-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="e21fc-117">Por ejemplo, si un cliente ha pagado 300 de un total de 500 dólares en una factura de venta, migramos la cantidad total de 500.</span><span class="sxs-lookup"><span data-stu-id="e21fc-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="e21fc-118">Si ha recibido pagos parciales, debe actualizarlos manualmente, antes o después de migrar los datos.</span><span class="sxs-lookup"><span data-stu-id="e21fc-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="e21fc-119">Le recomendamos que aplique las transacciones pendientes antes de migrar, simplemente para facilitar las cosas.</span><span class="sxs-lookup"><span data-stu-id="e21fc-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="e21fc-120">No migramos pedidos de compra o venta.</span><span class="sxs-lookup"><span data-stu-id="e21fc-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="e21fc-121">Antes de comenzar</span><span class="sxs-lookup"><span data-stu-id="e21fc-121">Before you start</span></span>
<span data-ttu-id="e21fc-122">Una parte importante del proceso de migración es especificar las cuentas a las que se deben migrar las transacciones.</span><span class="sxs-lookup"><span data-stu-id="e21fc-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="e21fc-123">Conviene planificar esta asignación antes de migrar los datos.</span><span class="sxs-lookup"><span data-stu-id="e21fc-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="e21fc-124">Por ejemplo, las cuentas en la que registre transacciones de:</span><span class="sxs-lookup"><span data-stu-id="e21fc-124">For example, the accounts where you post transactions for:</span></span>  
  
* <span data-ttu-id="e21fc-125">La venta de productos o servicios a los clientes.</span><span class="sxs-lookup"><span data-stu-id="e21fc-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="e21fc-126">La compra de productos o servicios a proveedores.</span><span class="sxs-lookup"><span data-stu-id="e21fc-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="e21fc-127">Ajustes en el libro mayor.</span><span class="sxs-lookup"><span data-stu-id="e21fc-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="e21fc-128"> requiere que las cuentas del libro mayor tengan números de cuenta asignados.</span><span class="sxs-lookup"><span data-stu-id="e21fc-128"> requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="e21fc-129">Asegúrese de que los números de cuenta están asignados a las cuentas de QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="e21fc-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="e21fc-130">Si las transacciones en QuickBooks Online tienen impuestos, debe configurar una cuenta de impuestos para sus jurisdicciones fiscales en [!INCLUDE[d365fin](includes/d365fin_md.md)] antes de poder registrar las transacciones.</span><span class="sxs-lookup"><span data-stu-id="e21fc-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="e21fc-131">¿Cómo empiezo a usar la extensión?</span><span class="sxs-lookup"><span data-stu-id="e21fc-131">How do I start using the extension?</span></span>
<span data-ttu-id="e21fc-132">Empezar es muy fácil.</span><span class="sxs-lookup"><span data-stu-id="e21fc-132">Getting started is easy.</span></span> <span data-ttu-id="e21fc-133">Únicamente tiene que ejecutar la guía de configuración asistida **Migración de datos**.</span><span class="sxs-lookup"><span data-stu-id="e21fc-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="e21fc-134">Instrucciones:</span><span class="sxs-lookup"><span data-stu-id="e21fc-134">Here's how:</span></span>

1. <span data-ttu-id="e21fc-135">Seleccione el ícono ![Buscar página o informe](media/ui-search/search_small.png "Buscar página o informe"), introduzca **Config. asistida** y, a continuación, seleccione **Migrar datos empresariales**.</span><span class="sxs-lookup"><span data-stu-id="e21fc-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="e21fc-136">Siga las instrucciones en cada paso de la guía de configuración asistida.</span><span class="sxs-lookup"><span data-stu-id="e21fc-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="e21fc-137">¿Qué hago después de la migración de datos?</span><span class="sxs-lookup"><span data-stu-id="e21fc-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="e21fc-138">Una vez haya migrado los datos, las transacciones muestran el estado **No registrado**, para que pueda revisarlas y crear ajustes.</span><span class="sxs-lookup"><span data-stu-id="e21fc-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="e21fc-139">Para revisar las transacciones, vaya a la página donde están normalmente.</span><span class="sxs-lookup"><span data-stu-id="e21fc-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="e21fc-140">Por ejemplo, para revisar facturas de ventas no registradas, vaya a la página **Facturas de ventas**.</span><span class="sxs-lookup"><span data-stu-id="e21fc-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="e21fc-141">Para revisar las diario de pagos, vaya a la página **Diario de pagos**.</span><span class="sxs-lookup"><span data-stu-id="e21fc-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="e21fc-142">Hay algunos pasos que es recomendable que haga:</span><span class="sxs-lookup"><span data-stu-id="e21fc-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="e21fc-143">Si las transacciones de QuickBooks Online tuvieran importes de descuento o de bonificación, deberá agregar manualmente los importes a las transacciones relacionadas en [!INCLUDE[d365fin](includes/d365fin_md.md)] antes de registrarlas.</span><span class="sxs-lookup"><span data-stu-id="e21fc-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="e21fc-144">Si está utilizando el impuesto sobre el valor añadido (IVA), es posible que tenga que agregar un grupo de contable de negocio y un grupo contable de productos a la configuración de grupos contables para poder contabilizar importes de IVA.</span><span class="sxs-lookup"><span data-stu-id="e21fc-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="e21fc-145">Verifique los saldos iniciales de las cuentas en el libro mayor.</span><span class="sxs-lookup"><span data-stu-id="e21fc-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="e21fc-146">QuickBooks Online no almacena el saldo actual de todas las cuentas, por lo que es posible que tenga que corregir los saldos iniciales.</span><span class="sxs-lookup"><span data-stu-id="e21fc-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="e21fc-147">Consulte también</span><span class="sxs-lookup"><span data-stu-id="e21fc-147">See Also</span></span>
[<span data-ttu-id="e21fc-148">Importar datos de empresa de otros sistemas financieros</span><span class="sxs-lookup"><span data-stu-id="e21fc-148">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="e21fc-149">[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] con extensiones](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e21fc-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
