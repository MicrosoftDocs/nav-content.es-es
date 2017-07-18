---
title: Libro mayor y plan de cuentas
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: es-es
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Libro mayor y plan de cuentas
La contabilidad almacena sus datos financieros y el plan de cuentas muestra las cuentas donde se registran todos los movimientos contables. Dynamics NAV incluye un gráfico estándar de cuentas que está preparado para respaldar su negocio.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Configuración de contabilidad y grupos contables
La contabilidad y la configuración de cómo los datos se registran en la contabilidad son la base de sus procesos empresariales.
En la ventana **Configuración contabilidad** especifique cómo gestionar determinados asuntos de contabilidad en su empresa. Esto incluye los detalles del redondeo de las facturas, los formatos de dirección y si desea usar una divisa adicional, por ejemplo.
De manera similar, en la ventana **Configuración grupos contables**, puede especificar cómo desea configurar las combinaciones generales del negocio y los grupos contables de producto. Rellene una línea por cada combinación de grupo contable de negocio y de producto.  

## <a name="the-chart-of-accounts"></a>Plan de cuentas
El plan de cuentas muestra todas las cuentas. Desde aquí, puede abrir los distintos informes que muestran los movimientos de contabilidad y saldo, y cerrar el balance. Desde cada cuenta, puede la ficha de cuenta y agregar o cambiar la configuración. También puede ver una lista de grupos contables que registran en dicha cuenta.  

Dynamics NAV impedirá que elimine una cuenta de contabilidad que guarde los datos que se necesitan en el plan de cuentas.  

## <a name="account-categories"></a>Categorías de cuenta
Con las categorías de cuenta puede asignar las cuentas contables a las categorías como personalización de la estructura de los informes financieros.  

La ventana **Categorías de cuenta** muestra las categorías y subcategorías principales existentes y las cuentas que asignó cada categoría. Puede crear nuevas subcategorías y asignarlas a las cuentas existentes.  

Puede agrupar las categorías de la cuenta marcando las subcategorías individuales. Esto le facilita la obtención de una descripción general, porque cada agrupación muestra un balance total. Por ejemplo, puede crear las subcategorías para distintos tipos de activos y a continuación crear grupos de categorías para los activos fijos y los activos circulantes. Puede crear un grupo de categorías marcando otras subcategorías debajo de una línea la ventana **Categorías de cuenta**.  

Para cada subcategoría puede especificar si las cuentas de esta categoría deben incluirse en los tipos específicos de informes financieros. Las categorías de cuentas ayudan a definir el diseño de sus balances financieros. Por ejemplo, el extracto de saldo predeterminado tiene un único movimiento para efectivo en activos. Si desea que el extracto del saldo tenga entradas secundarias de efectivo pequeño y de su cuenta corriente, puede agregar dos nuevas subcategorías, especificar la definición de informe adicional de Cuentas de efectivo para cada una de ellas y marcarlas debajo de la subcategoría de Efectivo. A continuación, cuando haya generado los esquemas de cuentas basados en sus cambios, su nuevo extracto de saldo mostrará un extracto total de efectivo y dos líneas con extractos para efectivo pequeño y cuenta corriente.     

##<a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)  
[Configure o cambie el plan de cuentas](finance-setup-setup-chart-accounts.md)  
[Esquemas de cuentas](finance-setup-account-schedule.md)  

