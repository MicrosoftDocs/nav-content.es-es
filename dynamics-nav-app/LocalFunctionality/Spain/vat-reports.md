---
title: Informes IVA
description: "El IVA se aplica a las transacciones que involucran bienes y servicios en España o bienes importados a España. La siguiente información proporciona más detalles sobre la funcionalidad de IVA."
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
ms.openlocfilehash: 9ceea78f6413201cb6201becfb93a9a06783fe8a
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="vat-reports"></a><span data-ttu-id="cb1c3-104">Informes IVA</span><span class="sxs-lookup"><span data-stu-id="cb1c3-104">VAT Reports</span></span>
<span data-ttu-id="cb1c3-105">El IVA se aplica a las transacciones que involucran bienes y servicios en España o bienes importados a España.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-105">VAT is charged on transactions that involve goods and services in Spain or goods imported into Spain.</span></span> <span data-ttu-id="cb1c3-106">La siguiente información proporciona más detalles sobre la funcionalidad de IVA.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-106">The following information provides more details about VAT functionality.</span></span>  
  
## <a name="equivalence-charge"></a><span data-ttu-id="cb1c3-107">Recargo de equivalencia</span><span class="sxs-lookup"><span data-stu-id="cb1c3-107">Equivalence Charge</span></span>  
 <span data-ttu-id="cb1c3-108">El impuesto de recargo de equivalencia (RE) se aplica a las actividades que no siguen las reglas del IVA.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-108">Equivalence Charge (EC) tax applies to activities that do not follow VAT rules.</span></span> <span data-ttu-id="cb1c3-109">Según las reglas RE, las empresas deben pagar un recargo a sus proveedores además del IVA.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-109">According to EC rules, companies must pay a surcharge to their vendors in addition to VAT.</span></span> <span data-ttu-id="cb1c3-110">Sin embargo, en las facturas de ventas sólo pueden cargar el IVA sin el recargo.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-110">However, they can only charge VAT without the surcharge on sales invoices.</span></span>  
  
### <a name="vat-with-ec-percentage"></a><span data-ttu-id="cb1c3-111">IVA con porcentaje RE</span><span class="sxs-lookup"><span data-stu-id="cb1c3-111">VAT with EC Percentage</span></span>  
 <span data-ttu-id="cb1c3-112">Los grupos de registro general predefinidos tienen un porcentaje RE, además de su porcentaje de IVA.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-112">Preset general posting groups have an EC percentage in addition to their VAT percentage.</span></span> <span data-ttu-id="cb1c3-113">Aunque el seguimiento del RE se efectúa por separado, los valores de ambos impuestos se fusionan con el IVA siempre que es posible.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-113">Although the EC is tracked separately, both tax values are merged with VAT when it is possible.</span></span> <span data-ttu-id="cb1c3-114">Si en la tabla de grupo contable el porcentaje RE es un campo independiente, el RE se fusiona con el valor de la columna **%IVA**.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-114">If the EC percentage is a separate field in the posting group, the EC is merged with the value in the **VAT %** column.</span></span>  
  
 <span data-ttu-id="cb1c3-115">Para imprimir libros de facturas emitidas y recibidas, el porcentaje de IVA y los porcentajes de RE se muestran en la tabla **Mov. IVA** durante el registro.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-115">For printing sales and purchase invoice books, the VAT percent and EC percentages are displayed in the **VAT Entry** table during posting.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="cb1c3-116">Si el artículo no tiene IVA gravable, se muestra automáticamente el número 0 en el campo **% IVA** en la ventana de información de IVA.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-116">If the item has no taxable VAT, 0 is automatically displayed in the **VAT %** field in the VAT information windows.</span></span>  
  
### <a name="telematic-vat"></a><span data-ttu-id="cb1c3-117">IVA Telemático</span><span class="sxs-lookup"><span data-stu-id="cb1c3-117">Telematic VAT</span></span>  
 <span data-ttu-id="cb1c3-118">Mediante el IVA telemático se pueden diseñar y generar los informes fiscales mensuales y anuales como archivos electrónicos o impresos.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-118">With telematic VAT you can design and generate monthly and yearly tax reports as electronic files or printed files.</span></span> <span data-ttu-id="cb1c3-119">Estos informes se pueden enviar a la administración fiscal a través de un programa externo o de un archivo XML del sitio Web de la administración.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-119">You can submit these reports to the tax authorities using a third-party program or an XML file from the tax authorities' website.</span></span>  
  
### <a name="vat-statement"></a><span data-ttu-id="cb1c3-120">Declaración IVA</span><span class="sxs-lookup"><span data-stu-id="cb1c3-120">VAT Statement</span></span>  
 <span data-ttu-id="cb1c3-121">La declaración de IVA muestra los importes e importes base de IVA en columnas diferentes.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-121">The VAT statement displays VAT amounts and base amounts in different columns.</span></span>  
  
 <span data-ttu-id="cb1c3-122">En la tabla **Nombre declar. IVA** hay dos tipos de plantillas de informe:</span><span class="sxs-lookup"><span data-stu-id="cb1c3-122">There are two report template types in the **VAT Statement Name** table:</span></span>  
  
-   <span data-ttu-id="cb1c3-123">**Informe 1 columna**</span><span class="sxs-lookup"><span data-stu-id="cb1c3-123">**One-Column Report**</span></span>  
  
-   <span data-ttu-id="cb1c3-124">**Informe 2 columnas**</span><span class="sxs-lookup"><span data-stu-id="cb1c3-124">**Two-Columns Report**</span></span>  
  
### <a name="vat-vies-declaration"></a><span data-ttu-id="cb1c3-125">IVA - declaración VIES</span><span class="sxs-lookup"><span data-stu-id="cb1c3-125">VAT-VIES Declaration</span></span>  
 <span data-ttu-id="cb1c3-126">Mediante IVA - declaración VIES se puede ejecutar un archivo por lotes para generar los informes de ventas de la Union Europea (UE).</span><span class="sxs-lookup"><span data-stu-id="cb1c3-126">With VAT-VIES declaration you can run a batch file to generate European Union (EU) sales reports.</span></span> <span data-ttu-id="cb1c3-127">El archivo por lotes exporta los movimientos al formato de archivo requerido para enviarlo a la aduana y a la administración fiscal.</span><span class="sxs-lookup"><span data-stu-id="cb1c3-127">The batch file exports the entries in the required file format for submission to customs and tax authorities.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="cb1c3-128">Consulte también</span><span class="sxs-lookup"><span data-stu-id="cb1c3-128">See Also</span></span>  
 <span data-ttu-id="cb1c3-129">[Funcionalidad local para España](spain-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="cb1c3-129">[Spain Local Functionality](spain-local-functionality.md) </span></span>  
 <span data-ttu-id="cb1c3-130">[Informe 340](report-340.md) </span><span class="sxs-lookup"><span data-stu-id="cb1c3-130">[Report 340](report-340.md) </span></span>  
 [<span data-ttu-id="cb1c3-131">Informe 347</span><span class="sxs-lookup"><span data-stu-id="cb1c3-131">Report 347</span></span>](report-347.md)