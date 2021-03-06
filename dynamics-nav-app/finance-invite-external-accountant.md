---
title: Agregar el contable externo a Dynamics NAV
description: "Obtenga información sobre cómo puede invitar a su contable externo a Dynamics NAV."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 09/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 856a95b929ca4fc419178c180bb8138e7f37ab61
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="inviting-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Invitación del contable externo a [!INCLUDE[d365fin](includes/d365fin_md.md)]
Si utiliza un contable externo para administrar los libros y los informes financieros, puede invitarle a su [!INCLUDE[d365fin](includes/d365fin_md.md)] para que pueda trabajar con usted en los datos fiscales.

Una vez que el contable ha accedido a su [!INCLUDE[d365fin](includes/d365fin_md.md)], puede utilizar el área de trabajo **Contable** que da acceso fácil a las ventanas más relevantes para el trabajo.  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a>Invitar al contable a [!INCLUDE[d365fin](includes/d365fin_md.md)]
En la última versión de [!INCLUDE[d365fin](includes/d365fin_md.md)], hemos facilitado la invitación a su contable externo. Abra simplemente la ventana **Usuarios**, y seleccione la acción **Invitar a contable externo** en la cinta de opciones. Se le crea un correo electrónico, ahora simplemente agregue el correo electrónico de trabajo de su contable y envíe la invitación.  

![Invitar al contable](./media/finance-invite-accountant/invite-accountant.png)

> [!TIP]  
>  Para ello es necesario que haya configurado el correo electrónico SMTP. Puede hacerlo usted mismo o preguntarle a su socio de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Además, debe iniciar sesión en [!INCLUDE[d365fin](includes/d365fin_md.md)] como administrador y no como propietario u otros usuarios.  

### <a name="separate-license"></a>Licencia independiente
En segundo plano, el contable se agrega a su suscriptor de Active Directory. Su administrador puede verificar que el contable acepta la invitación y se le asigna la licencia correcta. Los pasos para hacerlo dependen del tipo de cuenta que utilizó al registrarse en [!INCLUDE[d365fin](includes/d365fin_md.md)]. Este tema se basa en el uso de una cuenta de Office 365, que usa Microsoft Azure Active Directory.  

Si ha activado su suscripción de [!INCLUDE[d365fin](includes/d365fin_md.md)] y ya no utiliza la empresa de valoración, dispone de un suscriptor de Azure Active Directory. El administrador o el socio de [!INCLUDE[d365fin](includes/d365fin_md.md)] administra este suscriptor en el [portal de Azure](https://portal.azure.com). Aquí es donde se agregan nuevos usuarios y se aplican y se eliminan las licencias. Para obtener más información, vea el [resumen del portal de Microsoft Azure](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

Uno de los tipos de licencia para [!INCLUDE[d365fin](includes/d365fin_md.md)] es la licencia *Contable externo*. Este tipo de salida está pensado para que lo utilicen usuarios como, por ejemplo, contables externos. Esto significa que no tiene que comprar un puesto adicional en su Active Directory actual ni usar una de las cuentas de usuario de [!INCLUDE[d365fin](includes/d365fin_md.md)] existentes en el contable externo. Por ejemplo, si su suscripción de Office 365 actual incluye 10 usuarios para [!INCLUDE[d365fin](includes/d365fin_md.md)] y actualmente usa 10 licencias *Usuario completo*, el administrador puede agregar su contable externo como usuario invitado en el portal de Azure y asignarle la licencia *Contable externo* sin coste adicional. No obstante, solo puede tener un usuario con la licencia *Contable externo*. Si desea añadir más usuarios, debe actualizar su suscripción de Office 365 en consecuencia.  

## <a name="see-also"></a>Consulte también
[Finanzas](finance.md)  
[Configurar el correo electrónico manualmente o con la configuración asistida](madeira-how-setup-email.md)  
[Experiencias contables en Dynamics NAV](finance-accounting.md)  
[Dynamics NAV for Accountants en Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  

