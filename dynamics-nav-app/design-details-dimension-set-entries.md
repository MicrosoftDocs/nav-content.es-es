---
title: "Detalles de diseño: Movimientos de grupo de dimensiones"
description: "En esta documentación se proporciona información técnica detallada de los conceptos y los principios que se usan para rediseñar la característica de almacenamiento y registro de movimientos de dimensión."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, dimensions, codeunit
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8c285ae7af2fd6590f67e721c4e824f168528776
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-dimension-set-entries"></a><span data-ttu-id="2f1cd-103">Detalles de diseño: Movimientos de grupo de dimensiones</span><span class="sxs-lookup"><span data-stu-id="2f1cd-103">Design Details: Dimension Set Entries</span></span>
<span data-ttu-id="2f1cd-104">En esta documentación se proporciona información técnica detallada de los conceptos y los principios que se usan para rediseñar la característica de almacenamiento y registro de movimientos de dimensión en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2f1cd-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the dimension entry storing and posting feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="2f1cd-105">La documentación comienza con la descripción de la información general conceptual del rediseño.</span><span class="sxs-lookup"><span data-stu-id="2f1cd-105">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="2f1cd-106">A continuación, se explica la arquitectura técnica para mostrar cómo se realiza el rediseño.</span><span class="sxs-lookup"><span data-stu-id="2f1cd-106">Then it explains the technical architecture to show how the redesign is made.</span></span> <span data-ttu-id="2f1cd-107">Finalmente, proporciona ejemplos de código para preparar la migración y actualización del código de dimensión.</span><span class="sxs-lookup"><span data-stu-id="2f1cd-107">Finally, it provides code examples to prepare you for dimension code migration and upgrade.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="2f1cd-108">En esta sección</span><span class="sxs-lookup"><span data-stu-id="2f1cd-108">In This Section</span></span>  
[<span data-ttu-id="2f1cd-109">Información general de los movimientos del grupo dimensiones</span><span class="sxs-lookup"><span data-stu-id="2f1cd-109">Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)  
[<span data-ttu-id="2f1cd-110">Detalles de diseño: Búsqueda de combinaciones de dimensiones</span><span class="sxs-lookup"><span data-stu-id="2f1cd-110">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)  
[<span data-ttu-id="2f1cd-111">Detalles de diseño: Estructura de tablas</span><span class="sxs-lookup"><span data-stu-id="2f1cd-111">Design Details: Table Structure</span></span>](design-details-table-structure.md)  
[<span data-ttu-id="2f1cd-112">Detalles de diseño: Gestión de dimensiones de unidad de código 408</span><span class="sxs-lookup"><span data-stu-id="2f1cd-112">Design Details: Codeunit 408 Dimension Management</span></span>](design-details-codeunit-408-dimension-management.md)  
[<span data-ttu-id="2f1cd-113">Detalles de diseño: Ejemplos de código de patrones cambiados en las modificaciones</span><span class="sxs-lookup"><span data-stu-id="2f1cd-113">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
