---
title: "Crear plantillas para las declaraciones telemáticas de IVA en formato XML"
description: "Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios. Puede enviar los archivos en formato de texto y en formato XML. Este procedimiento describe cómo crear plantillas para los archivos XML."
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
ms.openlocfilehash: 30f5798425cf082b6361441e98feede6af58a68d
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-templates-for-telematic-vat-statements-in-xml-file-format"></a><span data-ttu-id="48c87-105">Crear plantillas para las declaraciones telemáticas de IVA en formato XML</span><span class="sxs-lookup"><span data-stu-id="48c87-105">How to: Create Templates for Telematic VAT Statements in XML File Format</span></span>
<span data-ttu-id="48c87-106">Para mostrar las declaraciones de IVA electrónicamente, debe crear plantillas para generar los archivos necesarios.</span><span class="sxs-lookup"><span data-stu-id="48c87-106">In order to submit VAT statements electronically, you must create templates to generate the required files.</span></span> <span data-ttu-id="48c87-107">Puede enviar los archivos en formato de texto y en formato XML.</span><span class="sxs-lookup"><span data-stu-id="48c87-107">You can submit files in text format and in XML format.</span></span> <span data-ttu-id="48c87-108">Este procedimiento describe cómo crear plantillas para los archivos XML.</span><span class="sxs-lookup"><span data-stu-id="48c87-108">This procedure describes how to create templates for XML files.</span></span>  
  
 <span data-ttu-id="48c87-109">Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).</span><span class="sxs-lookup"><span data-stu-id="48c87-109">For more information, see the [Spanish Tax Agency](http://go.microsoft.com/fwlink/?LinkID=238181) website.</span></span>  
  
### <a name="to-create-a-template-for-vat-statements-in-xml-file-format"></a><span data-ttu-id="48c87-110">Para crear una plantilla para las declaraciones telemáticas de IVA en formato de archivo XML</span><span class="sxs-lookup"><span data-stu-id="48c87-110">To create a template for VAT statements in XML file format</span></span>  
  
1.  <span data-ttu-id="48c87-111">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Declaración del IVA** y, a continuación, seleccione el vínculo apropiado.</span><span class="sxs-lookup"><span data-stu-id="48c87-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Statement**, and then choose the appropriate link.</span></span>  
  
2.  <span data-ttu-id="48c87-112">Seleccione la declaración de IVA requerida y luego, en la pestaña **Acciones**, elija **IVA telemático**, y **Diseñar archivo XML**.</span><span class="sxs-lookup"><span data-stu-id="48c87-112">Select the required VAT statement, and then, on the **Actions** tab, choose **Telematic VAT**, and then choose **Design XML file**.</span></span>  
  
3.  <span data-ttu-id="48c87-113">En la ventana **Formato transferencia XML**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="48c87-113">In the **XML Transference Format** window, fill in the fields as described in the following table.</span></span>  
  
    > [!IMPORTANT]  
    >  <span data-ttu-id="48c87-114">Los valores de los campos están determinados por las autoridades fiscales.</span><span class="sxs-lookup"><span data-stu-id="48c87-114">The values for the fields are determined by the tax authorities.</span></span>  
    >   
    >  <span data-ttu-id="48c87-115">Para obtener más información, consulte el sitio web de la [Agencia Tributaria](http://go.microsoft.com/fwlink/?LinkID=238181).</span><span class="sxs-lookup"><span data-stu-id="48c87-115">For more information, see the [Spanish Tax Agency](http://go.microsoft.com/fwlink/?LinkID=238181) website.</span></span>  
  
    |<span data-ttu-id="48c87-116">Campo</span><span class="sxs-lookup"><span data-stu-id="48c87-116">Field</span></span>|<span data-ttu-id="48c87-117">Description</span><span class="sxs-lookup"><span data-stu-id="48c87-117">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="48c87-118">**Nombre decl. IVA**</span><span class="sxs-lookup"><span data-stu-id="48c87-118">**VAT Stmt. Name**</span></span>|<span data-ttu-id="48c87-119">Especifique el nombre de la declaración del IVA para el que está diseñada esta plantilla.</span><span class="sxs-lookup"><span data-stu-id="48c87-119">Specify the VAT statement name that this template is for.</span></span>|  
    |<span data-ttu-id="48c87-120">**Nº**</span><span class="sxs-lookup"><span data-stu-id="48c87-120">**No.**</span></span>|<span data-ttu-id="48c87-121">Especifique el número de campo en el archivo de texto.</span><span class="sxs-lookup"><span data-stu-id="48c87-121">Specify the field number in the text file.</span></span>|  
    |<span data-ttu-id="48c87-122">**Tipo de línea**</span><span class="sxs-lookup"><span data-stu-id="48c87-122">**Line Type**</span></span>|<span data-ttu-id="48c87-123">Especifique si el tipo de línea de la declaración del IVA es un elemento XML o un atributo XML.</span><span class="sxs-lookup"><span data-stu-id="48c87-123">Specify whether the VAT statement line type is an XML element or an XML attribute.</span></span>|  
    |<span data-ttu-id="48c87-124">**Nivel sangría**</span><span class="sxs-lookup"><span data-stu-id="48c87-124">**Indentation Level**</span></span>|<span data-ttu-id="48c87-125">Especifique el nivel de sangría de la etiqueta.</span><span class="sxs-lookup"><span data-stu-id="48c87-125">Specify the indentation level for the label.</span></span> <span data-ttu-id="48c87-126">Este nivel se utiliza para formatear el archivo XML.</span><span class="sxs-lookup"><span data-stu-id="48c87-126">This level is used to format the XML file.</span></span>|  
    |<span data-ttu-id="48c87-127">**Nº línea maestro**</span><span class="sxs-lookup"><span data-stu-id="48c87-127">**Parent Line No.**</span></span>|<span data-ttu-id="48c87-128">Especifique el número de línea de la línea principal con la que se sangra la línea actual.</span><span class="sxs-lookup"><span data-stu-id="48c87-128">Specify the line number of the parent line that the current line is indented under.</span></span>|  
    |<span data-ttu-id="48c87-129">**Tipo de valor**</span><span class="sxs-lookup"><span data-stu-id="48c87-129">**Value Type**</span></span>|<span data-ttu-id="48c87-130">Especifique el subtipo del campo.</span><span class="sxs-lookup"><span data-stu-id="48c87-130">Specify the subtype of the field.</span></span><br /><br /> <span data-ttu-id="48c87-131">El subtipo especifica si la línea debe mostrar solo la parte entera de un importe, la parte decimal, o el importe total.</span><span class="sxs-lookup"><span data-stu-id="48c87-131">The subtype specifies if the line must show only the integer part of an amount, the decimal part, or the full amount.</span></span>|  
    |<span data-ttu-id="48c87-132">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="48c87-132">**Description**</span></span>|<span data-ttu-id="48c87-133">Especifique el texto que desea que aparezca en la etiqueta.</span><span class="sxs-lookup"><span data-stu-id="48c87-133">Specify the text that you want to appear on the label.</span></span>|  
    |<span data-ttu-id="48c87-134">**Valor**</span><span class="sxs-lookup"><span data-stu-id="48c87-134">**Value**</span></span>|<span data-ttu-id="48c87-135">Especifique el valor de la etiqueta.</span><span class="sxs-lookup"><span data-stu-id="48c87-135">Specify the value for the label.</span></span>|  
    |<span data-ttu-id="48c87-136">**Caja**</span><span class="sxs-lookup"><span data-stu-id="48c87-136">**Box**</span></span>|<span data-ttu-id="48c87-137">Especifique el número de casilla desde donde recuperar los datos.</span><span class="sxs-lookup"><span data-stu-id="48c87-137">Specify the box number from which to retrieve the data.</span></span>|  
    |<span data-ttu-id="48c87-138">**Preguntar**</span><span class="sxs-lookup"><span data-stu-id="48c87-138">**Ask**</span></span>|<span data-ttu-id="48c87-139">Especifica si el campo **Valor** se puede modificar antes de crear el archivo XML.</span><span class="sxs-lookup"><span data-stu-id="48c87-139">Specifies if the **Value** field can be changed before you create the XML file.</span></span>|  
    |<span data-ttu-id="48c87-140">**Existe importe**</span><span class="sxs-lookup"><span data-stu-id="48c87-140">**Exists Amount**</span></span>|<span data-ttu-id="48c87-141">Seleccione esta opción para incluir el importe existente.</span><span class="sxs-lookup"><span data-stu-id="48c87-141">Select to include the existing amount.</span></span>|  
  
4.  <span data-ttu-id="48c87-142">Repita el paso anterior para las líneas adicionales en la declaración de IVA.</span><span class="sxs-lookup"><span data-stu-id="48c87-142">Repeat the previous step for additional lines in the VAT statement.</span></span>  
  
5.  <span data-ttu-id="48c87-143">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="48c87-143">Choose the **OK** button.</span></span>  
  
 <span data-ttu-id="48c87-144">Esta acción crea la plantilla.</span><span class="sxs-lookup"><span data-stu-id="48c87-144">This creates the template.</span></span> <span data-ttu-id="48c87-145">Ahora puede crear un archivo que luego puede enviar a las autoridades fiscales.</span><span class="sxs-lookup"><span data-stu-id="48c87-145">Now, you can create a file that you can then submit to the tax authorities.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="48c87-146">Consulte también</span><span class="sxs-lookup"><span data-stu-id="48c87-146">See Also</span></span>  
 <span data-ttu-id="48c87-147">[Exportar declaraciones de IVA en formato XML](how-to-export-vat-statements-in-xml-format.md) </span><span class="sxs-lookup"><span data-stu-id="48c87-147">[How to: Export VAT Statements in XML Format](how-to-export-vat-statements-in-xml-format.md) </span></span>  
 <span data-ttu-id="48c87-148">[Crear plantillas para las declaraciones telemáticas de IVA en formato de archivo de texto](how-to-create-templates-for-telematic-vat-statements-in-text-file-format.md) </span><span class="sxs-lookup"><span data-stu-id="48c87-148">[How to: Create Templates for Telematic VAT Statements in Text File Format](how-to-create-templates-for-telematic-vat-statements-in-text-file-format.md) </span></span>  
 <span data-ttu-id="48c87-149">Formato XML de transferencia AEAT</span><span class="sxs-lookup"><span data-stu-id="48c87-149">AEAT Transference Format XML</span></span>