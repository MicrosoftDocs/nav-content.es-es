---
title: "Detalles de diseño: Coste de inventario"
description: "En esta documentación se proporciona información técnica detallada de los conceptos y los principios que se usan en las características de valoración de inventario en [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4b6db42020e62301bd882b679c2b6004374f0e49
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="64cbd-103">Detalles de diseño: Coste de inventario</span><span class="sxs-lookup"><span data-stu-id="64cbd-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="64cbd-104">En esta documentación se proporciona información técnica detallada de los conceptos y los principios que se usan en las características de valoración de inventario en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="64cbd-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="64cbd-105">La valoración de inventario, también conocida como "gestión de costes", se refiere al registro y la creación de informes sobre los costes operativos de la empresa.</span><span class="sxs-lookup"><span data-stu-id="64cbd-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="64cbd-106">En esta sección</span><span class="sxs-lookup"><span data-stu-id="64cbd-106">In This Section</span></span>  
[<span data-ttu-id="64cbd-107">Detalles de diseño: Métodos de coste</span><span class="sxs-lookup"><span data-stu-id="64cbd-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="64cbd-108">Detalles de diseño: Liquidación de productos</span><span class="sxs-lookup"><span data-stu-id="64cbd-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="64cbd-109">Detalles de diseño: Ajuste de coste</span><span class="sxs-lookup"><span data-stu-id="64cbd-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="64cbd-110">Detalles de diseño: Registro de coste previsto</span><span class="sxs-lookup"><span data-stu-id="64cbd-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="64cbd-111">Detalles de diseño: Coste medio</span><span class="sxs-lookup"><span data-stu-id="64cbd-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="64cbd-112">Detalles de diseño: Desviación</span><span class="sxs-lookup"><span data-stu-id="64cbd-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="64cbd-113">Detalles de diseño: Redondeo</span><span class="sxs-lookup"><span data-stu-id="64cbd-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="64cbd-114">Detalles de diseño: Componentes de coste</span><span class="sxs-lookup"><span data-stu-id="64cbd-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="64cbd-115">Detalles de diseño: Periodos de inventario</span><span class="sxs-lookup"><span data-stu-id="64cbd-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="64cbd-116">Detalles de diseño: Registro de inventario</span><span class="sxs-lookup"><span data-stu-id="64cbd-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="64cbd-117">Detalles de diseño: Registro de órdenes de producción</span><span class="sxs-lookup"><span data-stu-id="64cbd-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="64cbd-118">Detalles de diseño: Registro de pedidos de ensamblado</span><span class="sxs-lookup"><span data-stu-id="64cbd-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="64cbd-119">Detalles de diseño: Conciliación con contabilidad</span><span class="sxs-lookup"><span data-stu-id="64cbd-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="64cbd-120">Detalles de diseño: cuentas de contabilidad</span><span class="sxs-lookup"><span data-stu-id="64cbd-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="64cbd-121">Detalles de diseño: Revalorización</span><span class="sxs-lookup"><span data-stu-id="64cbd-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)
