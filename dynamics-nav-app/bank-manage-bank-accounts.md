---
title: Administrar cuentas bancarias
description: Debe reconciliar regularmente los movimientos de banco en Dynamics NAV con las transacciones bancarias relacionadas en sus cuentas bancarias.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: cd33af7062b5a8e75937f8750e09414f734d8c04
ms.contentlocale: es-es
ms.lasthandoff: 10/23/2017

---
# <a name="managing-bank-accounts"></a>Administrar cuentas bancarias
A intervalos regulares, debe conciliar sus movimientos bancarios en [!INCLUDE[d365fin](includes/d365fin_md.md)] con las transacciones bancarias relacionadas a cuentas bancarias en su banco y, a continuación, registrar el saldo en su cuenta bancaria. Puede realizar esta tarea, ya sea como parte del procesamiento de los pagos representados en un extracto bancario en el **Diario de conciliación de pagos**. O, de forma alternativa, puede realizar la tarea por separado del procesamiento de los pagos, en la ventana **Conciliación de cuentas bancarias** que admite movimientos de cheque. En ambos casos, puede rellenar las ventanas importando el extracto bancario a [!INCLUDE[d365fin](includes/d365fin_md.md)].

A veces, debe transferir importes entre la cuentas bancarias en [!INCLUDE[d365fin](includes/d365fin_md.md)] para reflejar las transferencias en su cuenta bancaria. Puede realizar esta tarea en la ventana **Diario general**, de diferentes maneras en función de la divisa de los fondos.

Para poder gestionar las cuentas bancarias, debe configurar cada cuenta bancaria como una ficha de banco. Además, debe configurar los servicios electrónicos que pueda usar para importar extractos bancarios y exportar archivos de pagos. Para obtener más información, consulte [Configurar cuentas bancarias](bank-setup-banking.md).

En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.

| Para | Vea |
| --- | --- |
| Concilie cuentas bancarias relacionadas en relación con el procesamiento de pagos en la ventana **Diario de conciliación de pagos**. |[Liquidación de pagos automáticamente y conciliación de cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Concilie cuentas bancarias, incluidos los movimientos de cheque, como una tarea independiente en la ventana **Conciliación de cuentas bancarias**. |[Conciliar cuentas bancarias](bank-how-reconcile-bank-accounts-separately.md) |
| Registre transferencias entre bancos en la misma divisa o en divisas diferentes. |[Transferir fondos bancarios](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a>Consulte también
[Configurar banca](bank-setup-banking.md)  
[Administrar cobros](receivables-manage-receivables.md)  
[Administrar pagos](payables-manage-payables.md)    
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Funciones empresariales generales](ui-across-business-areas.md)  

