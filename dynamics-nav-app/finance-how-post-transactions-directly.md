---
title: Registrar gastos o ingresos directamente en contabilidad
description: "Para las actividades empresariales que no está representadas por un documento, como los gastos o recibos de efectivo más pequeños, puede crear las transacciones relacionadas registrando líneas de diario en la ventana Diario general."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 06/28/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fc87a8111eb1383985816eb5901c714bbe1ccac1
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-transactions-directly-to-the-general-ledger"></a>Registrar transacciones directamente en la contabilidad
La mayoría de las transacciones financieras se registran en la contabilidad a través de documentos empresariales dedicados, como facturas de compra y pedidos de ventas. Para las actividades empresariales que no está representadas por un documento en [!INCLUDE[d365fin](includes/d365fin_md.md)], como los gastos o recibos de efectivo más pequeños, puede crear las transacciones relacionadas registrando líneas de diario en la ventana **Diario general**.

El diario general normalmente se utiliza para publicar los gastos propios de los empleados durante actividades comerciales, para su posterior reembolso. Para obtener más información, consulte [Procedimiento: registro y reembolso de los costes de los empleados](finance-how-record-reimburse-employee-expenses.md).

Los diarios generales registran las transacciones financieras directamente en cuentas contables y otras cuentas, como bancarias, de clientes, de proveedores y de empleados. Registrar con un diario general siempre crea movimientos en cuentas contables. Esto es así incluso si, por ejemplo, una línea del diario se registra en una cuenta de cliente, pues un movimiento se registra en una cuenta de cobros de contabilidad a través de un grupo de registro. Puede personalizar la versión de un diario general configurando una sección o una plantilla de diario. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).

A diferencia de los movimientos que se registran en documentos, que requieren un proceso de abono, puede revertir correctamente los movimientos que se registran con el diario general. Para obtener más información, consulte [Revertir registros](finance-how-reverse-journal-posting.md).

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a>Para registrar una transacción directamente en una cuenta contable
1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), especifique **Diarios generales** y elija el vínculo relacionado.
2. Abra la sección del diario general correspondiente. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).
3. En una línea nueva de diario, rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    
4. Repita el paso 3 para todas las transacciones independientes que desee registrar.

    > [!TIP]  
    > Si desea introducir varias líneas de transacción sobre una línea de cuenta de contrapartida, por ejemplo, de una cuenta bancaria, seleccione la casilla de verificación **Sugerir importe de compensación** en la línea de la sección en la ventana **Secciones diario general**. El campo **Importe** de la línea de la cuenta de contrapartida se rellena previamente de forma automática con el valor que se requiere para compensar las transacciones.
5. Seleccione la acción **Registrar** para registrar las transacciones en las cuentas contables especificadas.

## <a name="see-also"></a>Consulte también
[Trabajar con diarios generales](ui-work-general-journals.md)  
[Procedimiento: registro y reembolso de los costes de los empleados](finance-how-record-reimburse-employee-expenses.md)  
[Revertir registros](finance-how-reverse-journal-posting.md)  
[Finanzas](finance.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

