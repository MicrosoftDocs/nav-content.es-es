---
title: Recargo de equivalencia (RE)
description: "Un recargo de equivalencia (RE) es un impuesto que se utiliza en ventas minoristas y en actividades que no siguen las reglas del IVA. Según las reglas RE, las empresas deben pagar un recargo a sus proveedores al adquirir bienes además del IVA normal. Sin embargo, al vender bienes, solo puede cargarse el IVA. Algunos grupos de registro general deben tener un porcentaje RE, además del porcentaje de IVA. Esta información se efectúa por separado, pero para minimizar los cambios, ambos impuestos se combinan."
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
ms.openlocfilehash: bfa4accceb0f3ce42d9537602802492924127c28
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="equivalence-charges-ec"></a><span data-ttu-id="2a15c-107">Recargo de equivalencia (RE)</span><span class="sxs-lookup"><span data-stu-id="2a15c-107">Equivalence Charges (EC)</span></span>
<span data-ttu-id="2a15c-108">Un recargo de equivalencia (RE) es un impuesto que se utiliza en ventas minoristas y en actividades que no siguen las reglas del IVA.</span><span class="sxs-lookup"><span data-stu-id="2a15c-108">An Equivalence Charge (EC) is a tax that is used in retail sales and in activities that do not follow VAT rules.</span></span> <span data-ttu-id="2a15c-109">Según las reglas RE, las empresas deben pagar un recargo a sus proveedores al adquirir bienes además del IVA normal.</span><span class="sxs-lookup"><span data-stu-id="2a15c-109">Under EC rules, companies must pay a surcharge to their vendors when purchasing goods, in addition to the usual VAT.</span></span> <span data-ttu-id="2a15c-110">Sin embargo, al vender bienes, solo puede cargarse el IVA.</span><span class="sxs-lookup"><span data-stu-id="2a15c-110">However, when selling goods, only VAT can be charged.</span></span> <span data-ttu-id="2a15c-111">Algunos grupos de registro general deben tener un porcentaje RE, además del porcentaje de IVA.</span><span class="sxs-lookup"><span data-stu-id="2a15c-111">Some general posting groups must have an EC percentage in addition to the VAT percentage.</span></span> <span data-ttu-id="2a15c-112">Esta información se efectúa por separado, pero para minimizar los cambios, ambos impuestos se combinan.</span><span class="sxs-lookup"><span data-stu-id="2a15c-112">This information is tracked separately, but in order to minimize changes, both taxes are usually combined.</span></span>  
  
 <span data-ttu-id="2a15c-113">El campo **% RE** es un campo independiente en las tablas **Lín. compra**, **Lín. venta**, **Archivo lín. venta** y **Archivo lín. compra** .</span><span class="sxs-lookup"><span data-stu-id="2a15c-113">The **EC %** field is a separate field in the **Purchase Line**, **Sales Line**, **Sales Line Archive** and **Purchase Line Archive** tables.</span></span> <span data-ttu-id="2a15c-114">No obstante, en las líneas de ventas y compras, se combinan ambos impuestos y el valor se muestra en el campo **% IVA**.</span><span class="sxs-lookup"><span data-stu-id="2a15c-114">However, in sales and purchase lines, both taxes are combined and the value is displayed in the **VAT %** field.</span></span> <span data-ttu-id="2a15c-115">Se utiliza el campo **% IVA + RE** cuando se combinan las opciones de configuración.</span><span class="sxs-lookup"><span data-stu-id="2a15c-115">The **VAT + EC %** field is used when these values are combined.</span></span> <span data-ttu-id="2a15c-116">En el momento de la publicación, el porcentaje de IVA y el porcentaje de RE se insertan en la tabla de **Movs. IVA**.</span><span class="sxs-lookup"><span data-stu-id="2a15c-116">At the time of posting, the VAT percentage and the EC percentage are inserted in the **VAT Entry** table.</span></span> <span data-ttu-id="2a15c-117">Esto permite imprimir el informe **Libro facturas emitidas** y el informe **Libro facturas recibidas**.</span><span class="sxs-lookup"><span data-stu-id="2a15c-117">This makes it possible to print the **Sales Invoice Book** report and the **Purchases Invoice Book** report.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2a15c-118">Consulte también</span><span class="sxs-lookup"><span data-stu-id="2a15c-118">See Also</span></span>  
 <span data-ttu-id="2a15c-119">Usar para pagos electrónicos</span><span class="sxs-lookup"><span data-stu-id="2a15c-119">Use For Electronic Payments</span></span>   
 <span data-ttu-id="2a15c-120">Porcentaje de IVA</span><span class="sxs-lookup"><span data-stu-id="2a15c-120">VAT Percentage</span></span>   
 <span data-ttu-id="2a15c-121">Porcentaje de IVA</span><span class="sxs-lookup"><span data-stu-id="2a15c-121">VAT Percentage</span></span>
