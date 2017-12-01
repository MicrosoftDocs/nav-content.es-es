---
title: "Detalles de diseño: Gestión de dimensiones de unidad de código 408"
description: "La gestión de dimensiones de la unidad de código 408 corresponde a una biblioteca de funciones que controla tareas comunes relacionadas con las dimensiones, como copiar desde una tabla a otra o desde un documento a otro."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: aabc2ce0f52d4a551cf47ae0b82e3482936ddeab
ms.contentlocale: es-es
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="8bf38-103">Detalles de diseño: Gestión de dimensiones de unidad de código 408</span><span class="sxs-lookup"><span data-stu-id="8bf38-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="8bf38-104">La gestión de dimensiones de la unidad de código 408 corresponde a una biblioteca de funciones que controla tareas comunes relacionadas con las dimensiones, como copiar desde una tabla a otra o desde un documento a otro.</span><span class="sxs-lookup"><span data-stu-id="8bf38-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="8bf38-105">En este tema se enumeran las funciones que se han modificado en Microsoft Dynamics NAV 2013 R2 y se especifica qué se tiene que hacer en las funciones.</span><span class="sxs-lookup"><span data-stu-id="8bf38-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="8bf38-106">Muchas funciones se eliminan porque no es necesario realizar la copia entre tablas de dimensiones.</span><span class="sxs-lookup"><span data-stu-id="8bf38-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="8bf38-107">Funciones modificadas</span><span class="sxs-lookup"><span data-stu-id="8bf38-107">Modified Functions</span></span>  

|<span data-ttu-id="8bf38-108">Nombre de función</span><span class="sxs-lookup"><span data-stu-id="8bf38-108">Function Name</span></span>|<span data-ttu-id="8bf38-109">Descripción de la modificación</span><span class="sxs-lookup"><span data-stu-id="8bf38-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="8bf38-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="8bf38-111">Nueva función que sustituye a otras funciones de comprobación y acepta un identificador de grupo de dimensiones como argumento en lugar de una tabla de dimensiones.</span><span class="sxs-lookup"><span data-stu-id="8bf38-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="8bf38-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="8bf38-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="8bf38-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="8bf38-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="8bf38-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="8bf38-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="8bf38-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="8bf38-117">CheckDimValueComb</span></span>|<span data-ttu-id="8bf38-118">Eliminar.</span><span class="sxs-lookup"><span data-stu-id="8bf38-118">Delete.</span></span> <span data-ttu-id="8bf38-119">Todo el uso debe cambiar a CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="8bf38-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="8bf38-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-120">GetDefaultDim</span></span>|<span data-ttu-id="8bf38-121">Modificar para devolver un identificador entero de grupo de dimensiones en vez de un conjunto de registros.</span><span class="sxs-lookup"><span data-stu-id="8bf38-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="8bf38-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="8bf38-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="8bf38-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="8bf38-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="8bf38-126">Modificar para trabajar con DimSetID - > ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="8bf38-127">Funciones eliminadas</span><span class="sxs-lookup"><span data-stu-id="8bf38-127">Deleted Functions</span></span>  
 <span data-ttu-id="8bf38-128">Las funciones que se han eliminado de la unidad de código 408 en relación con los movimientos de grupo de dimensiones se presentan a continuación.</span><span class="sxs-lookup"><span data-stu-id="8bf38-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="8bf38-129">Durante la actualización del código de aplicación desde Microsoft Dynamics NAV 2009 o versiones anteriores a Microsoft Dynamics NAV 2016, las funciones siguientes no están disponibles en Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="8bf38-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="8bf38-130">Si tiene personalizaciones que utilizan una o varias de las funciones, debe actualizar ese código según corresponda.</span><span class="sxs-lookup"><span data-stu-id="8bf38-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="8bf38-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="8bf38-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="8bf38-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="8bf38-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="8bf38-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-136">InsertDocDim</span></span>  

 <span data-ttu-id="8bf38-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="8bf38-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="8bf38-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="8bf38-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="8bf38-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-141">InsertServContractDim</span></span>  

 <span data-ttu-id="8bf38-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="8bf38-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="8bf38-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="8bf38-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-144">GetDocDim</span></span>  

 <span data-ttu-id="8bf38-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-145">GetProdDocDim</span></span>  

 <span data-ttu-id="8bf38-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="8bf38-146">TypeToTableID1</span></span>  

 <span data-ttu-id="8bf38-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="8bf38-147">TypeToTableID2</span></span>  

 <span data-ttu-id="8bf38-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="8bf38-148">TypeToTableID3</span></span>  

 <span data-ttu-id="8bf38-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="8bf38-149">TypeToTableID4</span></span>  

 <span data-ttu-id="8bf38-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="8bf38-150">TypeToTableID5</span></span>  

 <span data-ttu-id="8bf38-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-152">DeleteDocDim</span></span>  

 <span data-ttu-id="8bf38-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="8bf38-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="8bf38-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="8bf38-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="8bf38-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="8bf38-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-160">ShowDocDim</span></span>  

 <span data-ttu-id="8bf38-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-161">SaveDocDim</span></span>  

 <span data-ttu-id="8bf38-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="8bf38-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="8bf38-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-164">ShowTempDim</span></span>  

 <span data-ttu-id="8bf38-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-165">SaveTempDim</span></span>  

 <span data-ttu-id="8bf38-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="8bf38-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="8bf38-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-168">SaveServContractDim</span></span>  

 <span data-ttu-id="8bf38-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="8bf38-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="8bf38-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="8bf38-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="8bf38-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="8bf38-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="8bf38-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="8bf38-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="8bf38-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="8bf38-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="8bf38-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="8bf38-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="8bf38-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="8bf38-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="8bf38-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="8bf38-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="8bf38-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="8bf38-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="8bf38-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="8bf38-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="8bf38-198">TestDimValue</span></span>  

 <span data-ttu-id="8bf38-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="8bf38-199">TestNewDimValue</span></span>  

 <span data-ttu-id="8bf38-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="8bf38-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="8bf38-201">(Eliminar porque se elimina la tabla ItemBudgetDim).</span><span class="sxs-lookup"><span data-stu-id="8bf38-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="8bf38-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-202">GetServContractDim</span></span>  

 <span data-ttu-id="8bf38-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="8bf38-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="8bf38-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="8bf38-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="8bf38-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="8bf38-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="8bf38-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="8bf38-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="8bf38-207">Consulte también</span><span class="sxs-lookup"><span data-stu-id="8bf38-207">See Also</span></span>
 <span data-ttu-id="8bf38-208">[Detalles de diseño: Movimientos de grupo de dimensiones](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="8bf38-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="8bf38-209">[Detalles de diseño: Resumen de Movimientos de grupo de dimensiones](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="8bf38-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="8bf38-210">[Detalles de diseño: Búsqueda de combinaciones de dimensiones](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="8bf38-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="8bf38-211">[Detalles de diseño: Estructura de tablas](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="8bf38-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="8bf38-212">Detalles de diseño: Ejemplos de código de patrones cambiados en las modificaciones</span><span class="sxs-lookup"><span data-stu-id="8bf38-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

