---
title: "Detalles de diseño: Gestión de almacén"
description: "En este tema se ofrece un resumen de los diseños, conceptos y principios que están detrás de las características de gestión de almacén en [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c86c44fbd183fbbec1a81e16394a352dbe0d2914
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-warehouse-management"></a><span data-ttu-id="76293-103">Detalles de diseño: Gestión de almacén</span><span class="sxs-lookup"><span data-stu-id="76293-103">Design Details: Warehouse Management</span></span>
<span data-ttu-id="76293-104">En esta documentación se ofrece un resumen de los conceptos y los principios que se usan en las características de gestión de almacén en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="76293-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="76293-105">Explica el diseño de las funciones de almacén central y cómo se integra el almacén con otras funciones de la cadena de aprovisionamiento.</span><span class="sxs-lookup"><span data-stu-id="76293-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span></span>  

<span data-ttu-id="76293-106">Para distinguir los distintos niveles de complejidad del almacenamiento, esta documentación se divide en dos grupos generales, configuraciones básicas y avanzadas de almacén, lo cual se indica mediante los títulos de sección.</span><span class="sxs-lookup"><span data-stu-id="76293-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span></span> <span data-ttu-id="76293-107">Esta diferenciación sencilla abarca diferentes niveles de complejidad, tal como se define mediante los módulos de producto y de ubicación.</span><span class="sxs-lookup"><span data-stu-id="76293-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span></span> <span data-ttu-id="76293-108">Para obtener más información, consulte [Detalles de diseño: Configuración almacén](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="76293-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="76293-109">En esta sección</span><span class="sxs-lookup"><span data-stu-id="76293-109">In This Section</span></span>  
[<span data-ttu-id="76293-110">Detalles de diseño: Resumen de almacén</span><span class="sxs-lookup"><span data-stu-id="76293-110">Design Details: Warehouse Overview</span></span>](design-details-warehouse-overview.md)  
[<span data-ttu-id="76293-111">Detalles de diseño: Configuración de almacén</span><span class="sxs-lookup"><span data-stu-id="76293-111">Design Details: Warehouse Setup</span></span>](design-details-warehouse-setup.md)  
[<span data-ttu-id="76293-112">Detalles de diseño: Flujo de entrada en almacén</span><span class="sxs-lookup"><span data-stu-id="76293-112">Design Details: Inbound Warehouse Flow</span></span>](design-details-inbound-warehouse-flow.md)  
[<span data-ttu-id="76293-113">Detalles de diseño: Flujos de almacén internos</span><span class="sxs-lookup"><span data-stu-id="76293-113">Design Details: Internal Warehouse Flows</span></span>](design-details-internal-warehouse-flows.md)  
[<span data-ttu-id="76293-114">Detalles de diseño: Disponibilidad en el almacén</span><span class="sxs-lookup"><span data-stu-id="76293-114">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="76293-115">Detalles de diseño: Flujo de salida del almacén</span><span class="sxs-lookup"><span data-stu-id="76293-115">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="76293-116">Detalles de diseño: Integración con inventario</span><span class="sxs-lookup"><span data-stu-id="76293-116">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)
