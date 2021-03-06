---
title: "Detalles de diseño: Cambios en la unidad de código 12: Cambios en los procedimientos de registro en el diario general"
description: "En esta versión de [!INCLUDE[d365fin](includes/d365fin_md.md)] se han implementado los siguientes cambios."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 19bbc6eb4939fa7f4e0180a62b03998cd2f386b6
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="codeunit-12-changes-changes-in-general-journal-post-procedures"></a>Cambios en la unidad de código 12: cambios en los procedimientos de registro en el diario general
En esta versión de [!INCLUDE[d365fin](includes/d365fin_md.md)] se han implementado los siguientes cambios.  

|**Microsoft Dynamics NAV 2009 R2**|**Microsoft Dynamics NAV 2013 R2**|**Comentario**|  
|----------------------------------------|----------------------------------------|-----------------|  
|GetGLReg|GetGLReg|Actualizado|  
|RunWithCheck|RunWithCheck|Actualizada|  
|RunWithoutCheck|RunWithoutCheck|Actualizada|  
|Code|Code|Actualizada|  
||PostGenJnlLine|Añadido|  
||InitAmounts|Añadido|  
||InitLastDocDate|Añadido|  
|InitVAT|InitVAT|Actualizada|  
|PostVAT|PostVAT|Actualizada|  
|InsertVAT|InsertVAT|Actualizada|  
|SummarizeVAT|SummarizeVAT|Actualizada|  
|InsertSummarizedVAT|InsertSummarizedVAT|Actualizada|  
|PostGLAcc|PostGLAcc|Actualizada|  
|PostCust|PostCust|Actualizada|  
|PostVend|PostVend|Actualizada|  
|PostBankAcc|PostBankAcc|Actualizada|  
|PostFixedAsset|PostFixedAsset|Actualizada|  
|PostICPartner|PostICPartner|Actualizada|  
|InitCodeUnit|StartPosting|Actualizada|  
||ContinuePosting|Añadido|  
|FinishCodeunit|FinishPosting|Actualizada|  
||PostUnrealizedVAT|Añadido|  
||CheckPostUnrealizedVAT|Añadido|  
||ExchangeAccounts|Añadido|  
|InitGLEntry|InitGLEntry|Actualizada|  
||InitGLEntryVAT|Añadido|  
||InitGLEntryVATCopy|Añadido|  
|InsertGLEntry|InsertGLEntry|Actualizada|  
||CreateGLEntry|Añadido|  
||CreateGLEntryBalAcc|Añadido|  
||CreateGLEntryVAT|Añadido|  
||CreateGLEntryVATCollectAdj|Añadido|  
||CreateGLEntryFromVATEntry|Añadido|  
||UpdateCheckAmounts|Añadido|  
|ApplyCustLedgEntry|ApplyCustLedgEntry|Actualizada|  
||CalcPmtDiscPossible|Añadido|  
||CalcPmtTolerancePossible|Añadido|  
|CalcPmtTolerance|CalcPmtTolerance|Actualizada|  
|CalcPmtDisc|CalcPmtDisc|Actualizada|  
|CalcPmtDiscIfAdjVAT|CalcPmtDiscIfAdjVAT|Actualizada|  
|CalcPmtDiscTolerance|CalcPmtDiscTolerance|Actualizada|  
||CalcPmtDiscVATBases|Añadido|  
||CalcPmtDiscVATAmounts|Añadido|  
||InsertPmtDiscVATForVATEntry|Añadido|  
||InsertPmtDiscVATForGLEntry|Añadido|  
|CalcCurrencyApplnRounding|CalcCurrencyApplnRounding|Actualizada|  
|FindAmtForAppln|FindAmtForAppln|Actualizada|  
|CalcCurrencyUnrealizedGainLoss|CalcCurrencyUnrealizedGainLoss|Actualizada|  
|CalcCurrencyRealizedGainLoss|CalcCurrencyRealizedGainLoss|Actualizada|  
|CalcApplication|CalcApplication|Actualizada|  
|CalcRemainingPmtDisc|CalcRemainingPmtDisc|Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CalcAmtLCYAdjustment|CalcAmtLCYAdjustment|Añadido|  
|InitNewCVLedgEntry|InitFromGenJnlLine|Desplazado a la tabla 383 Mem. inter. mov. CV detallado|  
|InitOldCVLedgEntry|CopyFromCVLedgEntryBuf|Desplazado a la tabla 383 Mem. inter. mov. CV detallado|  
|InsertDtldCVLedgEntry|InsertDtldCVLedgEntry|Desplazado a la tabla 383 Mem. inter. mov. CV detallado|  
||InitBankAccLedgEntry|Añadido|  
||InitCheckLedgEntry|Añadido|  
||InitCustLedgEntry|Añadido|  
||InitVendLedgEntry|Añadido|  
||InsertDtldCustLedgEntry|Añadido|  
||InsertDtldVendLedgEntry|Añadido|  
|CustUnrealizedVAT|CustUnrealizedVAT|Actualizada|  
|CustPostApplyCustLedgEntry|CustPostApplyCustLedgEntry|Actualizada|  
||PrepareTempCustLedgEntry|Añadido|  
|UnapplyCustLedgEntry|UnapplyCustLedgEntry|Actualizada|  
|TransferCustLedgEntry|CopyFromGenJnlLine|Desplazado a la tabla 21 Movimiento de cliente|  
|PostDtldCustLedgEntries|PostDtldCustLedgEntries|Actualizada|  
||PostDtldCustLedgEntry|Añadido|  
||PostDtldCustLedgEntryUnapply|Añadido|  
||GetDtldCustLedgEntryAccNo|Añadido|  
|ZeroTransNoDtldCustLedgEntries|SetZeroTransNo|Desplazado a la tabla 379 Movs. clientes detallados|  
|AutoEntrForDtldCustLedgEntries||Refactorizado a PostDtldCustLedgEntryUnapply|  
|CustUpdateDebitCredit|UpdateDebitCredit|Desplazado a la tabla 379 Movs. clientes detallados|  
|ApplyVendLedgEntry|ApplyVendLedgEntry|Actualizada|  
||PrepareTempVendLedgEntry|Añadido|  
|VendPostApplyVendLedgEntry|VendPostApplyVendLedgEntry|Actualizada|  
|UnapplyVendLedgEntry|UnapplyVendLedgEntry|Actualizada|  
|TransferVendLedgEntry|CopyFromGenJnlLine|Desplazado a la tabla 25 Movimiento de proveedor|  
|PostDtldVendLedgEntries|PostDtldVendLedgEntries|Actualizada|  
||PostDtldVendLedgEntry|Añadido|  
||PostDtldVendLedgEntryUnapply|Añadido|  
||GetDtldVendLedgEntryAccNo|Añadido|  
||PostDtldCVLedgEntry|Añadido|  
||PostDtldCustVATAdjustment|Añadido|  
||PostDtldVendVATAdjustment|Añadido|  
|ZeroTransNoDtldVendLedgEntries|SetZeroTransNo|Desplazado a la tabla 380 Movs. proveedores detallados|  
|AutoEntrForDtldVendLedgEntries||Refactorizado a PostDtldVendLedgEntryUnapply|  
|VendUpdateDebitCredit|UpdateDebitCredit|Desplazado a la tabla 380 Movs. proveedores detallados|  
|VendUnrealizedVAT|VendUnrealizedVAT|Actualizada|  
||PostUnrealVATEntry|Añadido|  
||PostApply|Añadido|  
|PostUnrealVATByUnapply|PostUnrealVATByUnapply|Actualizada|  
||PostUnapply|Añadido|  
||InsertDtldCustLedgEntryUnapply|Añadido|  
||InsertDtldVendLedgEntryUnapply|Añadido|  
||InsertTempVATEntry|Añadido|  
||ProcessTempVATEntry|Añadido|  
||UpdateCustLedgEntry|Añadido|  
||UpdateVendLedgEntry|Añadido|  
|UpdateCalcInterest|UpdateCalcInterest|Actualizada|  
|UpdateCalcInterest2|UpdateCalcInterest2|Actualizada|  
|GLCalcAddCurrency|GLCalcAddCurrency|Actualizada|  
|HandleAddCurrResidualGLEntry|HandleAddCurrResidualGLEntry|Actualizada|  
|CalcLCYToAddCurr|CalcLCYToAddCurr|Actualizada|  
|CalcAddCurrFactor||Eliminado|  
|GetCurrencyExchRate|GetCurrencyExchRate|Actualizada|  
|ExchAmount|ExchangeAmount|Desplazado a la tabla 330 Tipo cambio divisa|  
|ExchangeAmtLCYToFCY2|ExchangeAmtLCYToFCY2|Actualizada|  
|CalcAddCurrForUnapplication|CalcAddCurrForUnapplication|Actualizada|  
|CheckNonAddCurrCodeOccurred|CheckNonAddCurrCodeOccurred|Actualizada|  
|CheckCalcPmtDisc||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscCVCust||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscCust||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscGenJnlCust||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscCVVend||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscVend||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|CheckCalcPmtDiscGenJnlVend||Desplazado a unidad de código 426 Gestión de tolerancia de pago|  
|Reverse|Reverse|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ReverseCustLedgEntry|ReverseCustLedgEntry|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ReverseVendLedgEntry|ReverseVendLedgEntry|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ReverseBankAccLedgEntry|ReverseBankAccLedgEntry|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ReverseVAT|ReverseVAT|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|SetReversalDescription|SetReversalDescription|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ApplyCustLedgEntryByReversal|ApplyCustLedgEntryByReversal|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|ApplyVendLedgEntryByReversal|ApplyVendLedgEntryByReversal|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
|PostPmtDiscountVATByUnapply|PostPmtDiscountVATByUnapply|Desplazado a unidad de código 17 Diario gen.-Revertir registrado|  
||CheckDimComb|Añadido en unidad de código 17 Diario gen.-Revertir registrado|  
||CopyCustLedgEntry|Añadido en unidad de código 17 Diario gen.-Revertir registrado|  
||CopyVendLedgEntry|Añadido en unidad de código 17 Diario gen.-Revertir registrado|  
||CopyBankAccLedgEntry|Añadido en unidad de código 17 Diario gen.-Revertir registrado|  
|HandlDtlAddjustment|HandleDtldAdjustment|Actualizada|  
|CollectAddjustment|CollectAdjustment|Actualizada|  
|SetOverDimErr|SetOverDimErr|Actualizada|  
|PostJob|PostJob|Actualizada|  
|InsertVATEntriesFromTemp|InsertVATEntriesFromTemp|Actualizada|  
|CaptureOrRefundCreditCardPmnt|CaptureOrRefundCreditCardPmnt|Actualizada|  
|UpdateDOPaymentTransactEntry|UpdateDOPaymentTransactEntry|Actualizada|  
|ABSMin|ABSMin|Actualizada|  
|GetApplnRoundPrecision|GetApplnRoundPrecision|Actualizada|  
|CheckDimValueForDisposal|CheckDimValueForDisposal|Actualizada|  
|CalculateCurrentBalance|CalculateCurrentBalance|Actualizada|  
|IncludeVATAmount||Desplazado a la tabla 81 Lín. diario general|  
|CalcVATAmountFromVATEntry|CalcVATAmountFromVATEntry|Actualizada|  
||TotalVATAmountOnJnlLines|Añadido|  
||SetGLRegReverse|Añadido|  
||GetGLSetup|Añadido|  
||ReadGLSetup|Añadido|  
||CheckSalesExtDocNo|Añadido|  
||CheckPurchExtDocNo|Añadido|  
||CheckGLAccDimError|Añadido|  
||GetCurrency|Añadido|  
||PostDtldAdjustment|Añadido|  
||GetNextEntryNo|Añadido|  
||GetNextTransactionNo|Añadido|  
||GetNextVATEntryNo|Añadido|  
||IncrNextVATEntryNo|Añadido|  
||IsNotPayment|Añadido|  
||IsTempGLEntryBufEmpty|Añadido|  
||IsVATAdjustment|Añadido|  
||IsVATExcluded|Añadido|  
||UpdateDimensions|Añadido|  
||UpdateDimensionsFromCustLedgEntry|Añadido|  
||UpdateDimensionsFromVendLedgEntry|Añadido|  
||UpdateTotalAmounts|Añadido|  
||CreateGLEntriesForTotalAmounts|Añadido|  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Cambios en unidad de código 12: Asociación de variables globales para línea de registro en diario general](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)

