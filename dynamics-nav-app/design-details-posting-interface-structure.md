---
title: "Detalles de diseño: estructura de interfaz de registro"
description: Este tema proporciona un resumen de los procedimientos globales en la estructura de la interfaz de registro.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cc5efca8087bc24ab988ae592a9ba60e4caf46bb
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="0715f-103">Detalles de diseño: estructura de interfaz de registro</span><span class="sxs-lookup"><span data-stu-id="0715f-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="0715f-104">En la estructura de interfaz de registro de [!INCLUDE[d365fin](includes/d365fin_md.md)] existen varios procedimientos globales que utilizan la misma estructura:</span><span class="sxs-lookup"><span data-stu-id="0715f-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="0715f-105">RunWithCheck y RunWithoutCheck llaman al código de procedimiento - interfaz de registro genérica para la línea de diario general.</span><span class="sxs-lookup"><span data-stu-id="0715f-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="0715f-106">CustPostApplyCustLedgEntry: registrar aplicación de cliente, llamada desde la unidad de código 226 Mov. cliente-Liquidar movimientos registrados.</span><span class="sxs-lookup"><span data-stu-id="0715f-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="0715f-107">VendPostApplyVendLedgEntry: registrar liquidación de proveedor, llamada desde la unidad de código 227 Mov. proveedor-Liquidar movimientos registrados.</span><span class="sxs-lookup"><span data-stu-id="0715f-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="0715f-108">UnapplyCustLedgEntry: registrar desliquidación de liquidación de cliente, llamada desde la unidad de código 226 Mov. cliente-Liquidar movimientos registrados.</span><span class="sxs-lookup"><span data-stu-id="0715f-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="0715f-109">UnapplyVendLedgEntry: registrar desliquidación de liquidación de proveedor, llamada desde la unidad de código 227 Mov. proveedor-Liquidar movimientos registrados.</span><span class="sxs-lookup"><span data-stu-id="0715f-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0715f-110">Consulte también</span><span class="sxs-lookup"><span data-stu-id="0715f-110">See Also</span></span>  
[<span data-ttu-id="0715f-111">Detalles de diseño: estructura de motor de registro</span><span class="sxs-lookup"><span data-stu-id="0715f-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)