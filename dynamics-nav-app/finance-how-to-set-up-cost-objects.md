---
title: 'Procedimiento: configurar objetos de coste'
description: "Aprender cómo configurar los objetos de coste, que son parecidos a las dimensiones de contabilidad."
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
ms.openlocfilehash: 07c1d837f858641456fde84431e1a9695a992efe
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-cost-objects"></a>Procedimiento: configurar objetos de coste
Los objetos de coste son proyectos, productos o servicios de una empresa. El plan de objetos de coste es similar a la información de dimensión de contabilidad. Puede configurar el plan de objetos de coste de la siguiente forma:  

* Transfiera los valores de dimensión en la contabilidad al plan de objetos de coste. Puede hacer los ajustes necesarios después de la transferencia.  
* Cree un plan del objeto de coste que es independiente de la contabilidad o agregue un objeto de coste nuevo a un plan existente de objetos de coste. Debe crear cada objeto de coste por separado.  

## <a name="to-transfer-dimension-values-from-the-general-ledger-to-the-chart-of-cost-objects"></a>Para transferir valores de dimensión de la contabilidad al plan de objetos de coste  
1.  Configurar una dimensión para que sea la dimensión del objeto de coste en la ventana **Actualizar dimensiones CA**. Sólo los valores de esta dimensión se transfieren.  
2.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan objetos coste** y, a continuación, seleccione el vínculo relacionado.  
3.  Elija la acción **Traer objetos coste de dimensión** para transferir los valores de dimensión al plan de objetos de coste. La función transfiere los valores de dimensión que definió en el paso 1.  

    > [!NOTE]  
    >  Puede configurar el campo **Alinear dimensión objeto coste** para definir una sincronización unidireccional de los valores de dimensión de la contabilidad al plan de objetos de coste. No puede definir una sincronización del plan de objetos de coste a los valores de dimensión de la contabilidad.  

El plan de objetos de coste contendrá ahora todos los valores de dimensión especificados desde la contabilidad e incluirá títulos y subtotales.  

## <a name="to-create-new-cost-objects-in-the-chart-of-cost-objects-window"></a>Crear nuevos objetos de coste en la ventana Plan objetos coste  
Puede configurar y mantener objetos de coste en la ficha **Plan objeto de coste** o bien en la ventana **Plan objetos coste**. En este procedimiento, va a configurar objetos de coste en la ventana **Plan de objetos de coste**.  

1.  Abra la ventana **Plan objetos coste** en el modo de edición.  
2.  En el campo **Código**, introduzca el código del objeto de coste. Todos los objetos de coste deben disponer de un código.  
3.  En el campo **Nombre**, introduzca el nombre del objeto de coste.  
4.  Seleccione la flecha desplegable del campo **Tipo línea** para especificar la finalidad del objeto de coste.  

    * Para los objetos de coste de la línea **Total** debe rellenar el campo **Total desde/a**. Utilice el operador **or**, que es una línea vertical (**&#124;**), para establecer rangos de objetos de coste.  
    * Para objetos de coste del tipo de línea **Total final**, este campo se rellena automáticamente cuando utiliza la función Aplicar sangría.  
5.  Rellene el campo **Orden clasificación**.  
6.  Seleccione la siguiente línea vacía para crear un objeto de coste nuevo y, a continuación, repita del paso 2 al 5.  
7.  Cuando haya configurado todos los objetos de coste, elija la acción **Aplicar sangría a objetos coste**. Elija el botón **Sí**.  

> [!IMPORTANT]  
>  Si ha introducido definiciones en los campos **Total desde/a** para los objetos de coste de **Total final** antes de ejecutar la función Aplicar sangría, deberá volver a introducirlas. La función sobrescribe los valores de todos los campos de **Total final**.  

## <a name="see-also"></a>Consulte también  
[Contabilidad para costes](finance-manage-cost-accounting.md)  
[Definición de centros de coste y de objetos de coste para el plan de cuentas](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md)   
[Saldos entre el tipo de coste, centro de coste y objeto de coste](finance-balances-between-cost-type-cost-center-and-cost-object.md)   
[Configuración de contabilidad de costes](finance-set-up-cost-accounting.md)   
[Terminología en contabilidad de costes](finance-terminology-in-cost-accounting.md)   
[Acerca de la contabilidad de costes](finance-about-cost-accounting.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

