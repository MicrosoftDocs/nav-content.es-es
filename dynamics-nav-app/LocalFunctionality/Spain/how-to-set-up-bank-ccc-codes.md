---
title: "Configuración de códigos CCC de bancos"
description: "El Código Cuenta Cliente (CCC) es un código de cuenta único usado por los bancos para identificar a sus clientes. El código CCC se imprime en los documentos bancarios, como cheques y extractos."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: ef03ad7a9a38b4e5ac94f72e9074a94ae8388ef4
ms.contentlocale: es-es
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-set-up-bank-ccc-codes"></a>Configuración de códigos CCC de bancos
El Código Cuenta Cliente (CCC) es un código de cuenta único usado por los bancos para identificar a sus clientes. El código CCC se imprime en los documentos bancarios, como cheques y extractos.  

Se pueden configurar códigos CCC en las siguientes ubicaciones:  

- Ventana **Ficha banco**  
- Ventana **Información empresa**  
- Ventana **Ficha banco cliente**  
- Ventana **Ficha banco proveedor**  

El procedimiento siguiente describe cómo configurar códigos CCC de banco para su empresa.  

## <a name="to-enter-ccc-codes"></a>Para introducir códigos CCC  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Información de la empresa** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene los campos de la ficha desplegable **Pagos**, tal como se describe en la tabla siguiente.  

    |Campo|Description|  
    |---------------------------------|--------------|---------------------------------------|  
    |**CCC Cód. banco**|1-4|Identifica el banco en el que se ha abierto la cuenta.|  
    |**CCC Cód. oficina**|5-8|Identifica el código de la oficina. Si el banco no utiliza esta referencia, el código de la oficina pueden ser ceros.|  
    |**CCC Dígito control**|9-10|Identifica los dígitos de control.|  
    |**CCC Nº cuenta**|11-20 (España)<br /><br /> 11-21 (Portugal)|Identifica el número de cuenta, que se puede ajustar con ceros a la izquierda.|  

El siguiente procedimiento describe cómo configurar códigos bancarios CCC para cuentas bancarias de clientes existentes, pero los mismos pasos se aplican a proveedores, cuentas bancarias e información de la compañía.  

## <a name="to-set-up-bank-ccc-codes-for-a-customer-bank-account"></a>Para configurar códigos CCC de banco de un banco cliente  

1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Ficha banco cliente** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ficha desplegable **Transferencia**, escriba la información en los campos CCC relevantes.  

    > [!NOTE]  
    >  Debe configurar información de la empresa en la ficha desplegable **Pagos**.  

3.  Elija el botón **Aceptar**.  

## <a name="see-also"></a>Consulte también  
[Configurar cuentas bancarias](../../bank-how-setup-bank-accounts.md) 

