---
title: "Registro e impresión de todas las transacciones de un periodo"
description: "Las empresas deben enviar los movimientos de transacciones de su negocio, agrupados por números de transacción, en un informe anual a la administración fiscal. Cada transacción de contabilidad debe tener un número secuencial para el ejercicio. Al registrar las transacciones, se asignarán números de transacción a los movimientos de contabilidad."
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
ms.openlocfilehash: e5d1e2636e45dbdc6d1bc7ee3a2c9b8324f4a4f1
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-and-print-all-transactions-for-a-period"></a>Registro e impresión de todas las transacciones de un periodo
Las empresas deben enviar los movimientos de transacciones de su negocio, agrupados por números de transacción, en un informe anual a la administración fiscal. Cada transacción de contabilidad debe tener un número secuencial para el ejercicio. Al registrar las transacciones, se asignarán números de transacción a los movimientos de contabilidad.  
  
### <a name="to-post-all-transactions-for-a-period"></a>Para registrar todas las transacciones de un periodo  
  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diario general** y, a continuación, seleccione el vínculo relacionado.  
  
2.  Rellene los campos tal como se describe en la tabla siguiente.  
  
    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nombre sección**|Seleccione el nombre de sección del diario requerido.|  
    |**Nº asiento**|Escriba el número de transacción. **Nota**: Si la transacción está saldada, el siguiente número aparecerá automáticamente y los detalles de transacción relacionados aparecerán en la siguiente fila. Si la transacción no está saldada, aparecerá el mismo número de transacción con detalles de transacción relacionados.|  
  
3.  En la pestaña **Inicio**, en el grupo de acciones **Proceso**, elija **Registrar** y, a continuación elija el botón **Sí** para confirmar el registro.  
  
4.  Elija el botón **Aceptar**.  
  
     Una vez registrado el diario, se asigna un número de transacción final a los movimientos del diario. Este número es secuencial, sin discontinuidades. Por lo tanto, para cada ejercicio, todos los movimientos agrupados por su número de transacción se clasifican en orden secuencial, sin discontinuidades o espacios en blanco.  
  
### <a name="to-print-all-transactions-for-a-period"></a>Para imprimir todas las transacciones de un periodo  
  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Registro movs. contabilidad** y, a continuación, seleccione el vínculo relacionado.  
  
2.  Para definir el campo **Nº asiento periodo** para todos los movimientos de contabilidad del periodo en un orden secuencial, en la pestaña **Acciones** del grupo **Funciones** elija **Asignar nº asiento periodo**.  
  
3.  Seleccione los filtros apropiados.  
  
4.  Elija el botón **Aceptar**.  
  
    > [!NOTE]  
    >  Todas las transacciones se ordenan por fecha de registro y se asigna un número secuencial a cada movimiento del campo **Nº asiento periodo** .  
  
5.  En la ventana **Registro movs. contabilidad**, en la pestaña **Acciones** elija **Imprimir página**.  
  
## <a name="see-also"></a>Consulte también  
 [Números de transacción](transaction-numbers.md)
