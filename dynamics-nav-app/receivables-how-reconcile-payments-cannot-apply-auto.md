---
title: "Procedimiento: Conciliar pagos que no se pueden liquidar automáticamente"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f9fd7c2958aaa359d2f6af5dde2e8be81349e900
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-that-cannot-be-applied-automatically"></a>Procedimiento: Conciliar pagos que no se pueden liquidar automáticamente
En ocasiones es posible que tenga que gestionar los pagos en su cuenta bancaria que no se pueden liquidar con un cliente, proveedor o movimiento de cuenta bancario abierto relacionado. Los motivos pueden ser que no haya ningún documento en Dynamics NAV con el que se pueda liquidar el pago o el documento relacionado en Dynamics NAV tiene un importe diferente al de la transacción, por ejemplo, debido al tipo de cambio de divisa. En la ventana **Diario de conciliación de pagos**, todos los importes de transacciones de pagos que aún no se hayan liquidado aparecen en el campo **Diferencia**, incluidos los importes que no se pueden liquidar debido a los motivos que aparecen anteriormente.

Los pagos que no se pueden liquidar pueden aparecer en líneas de diario de conciliación de las distintas formas siguientes:

- El valor del campo **Diferencia** es igual al valor del campo **Importe de transacción**, que indica que no se puede liquidar ninguna parte del pago con el cliente, proveedor o movimiento de cuenta bancaria abierto relacionado.

- El valor del campo **Diferencia** es inferior al valor del campo **Importe de transacción**, que indica que no se puede liquidar ninguna parte del pago con el cliente, proveedor o movimiento de cuenta bancaria abierto relacionado. La parte del pago restante no se puede liquidar y se debe conciliar manualmente o registrándola directamente en una cuenta.

Para conciliar esos pagos, puede seleccionar el botón Transferir diferencia a cuenta y especificar en qué cuenta se registrará el importe del campo Diferencia al registrar el diario de conciliación de pagos.

**Nota**: Existen funciones similares para configurar la conciliación automática de pagos periódicos que no se pueden liquidar con el cliente, proveedor o movimiento de cuenta bancaria abierto relacionado. [Para más información, consulte Procedimiento: Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

## <a name="to-reconcile-payments-that-cannot-be-applied"></a>Para conciliar pagos que no se pueden liquidar
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de conciliación de pagos** y, a continuación, seleccione el enlace relacionado.
2. Abra un diario de conciliación de pagos. Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).
3. Seleccione **Transferir diferencia a cuenta**. Se abre la ventana **Transferir diferencia a cuenta**. se abre la ventana.
4. En el campo **Tipo de cuenta**, especifique el tipo de cuenta en el que se registrará el importe del pago.
5. En el campo **N.º cuenta** especifique la cuenta en la que se registrará el importe del pago.
6. En el campo **Descripción**, especifique el texto que describe este registro de pago directo. Por omisión, se inserta el texto del campo **Texto de la transacción** en la línea de diario de conciliación de pagos.
7. Elija el botón **Aceptar**.

Si el valor del campo **Diferencia** era igual al valor del campo **Importe de la transacción** cuando registró el diario de conciliación de pagos, el pago completo de la línea de diario se registrará directamente en la cuenta de contrapartida especificada.

Si el valor del campo **Diferencia** era inferior al valor del campo **Importe de la transacción**, se creará una línea de diario adicional con el mismo texto y fecha y con la diferencia insertada en el campo **Importe de la transacción**. En la línea del diario original, la diferencia se deducirá del valor del campo **Importe de la transacción** y el pago se liquidará con el cliente, proveedor o movimiento de cuenta bancaria relacionado. Cuando registre el diario de conciliación de pagos, se registrará una parte del pago como un pago liquidado. La otra parte del pago se registrará directamente en la cuenta especificada.

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)

