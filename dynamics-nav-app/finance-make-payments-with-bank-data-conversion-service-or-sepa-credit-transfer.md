---
title: "Seleccione el método de pagos electrónicos"
description: "Procese pagos a sus proveedores exportando un archivo junto con la información de pago desde las líneas de diario."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baafa833fb170fb05f866aac91a05085545aaf97
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a><span data-ttu-id="682b4-103">Realizar pagos con Servicio de conversión de datos del banco o Transferencia de crédito SEPA</span><span class="sxs-lookup"><span data-stu-id="682b4-103">Make Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>
<span data-ttu-id="682b4-104">En la ventana **Diario de pagos**, puede procesar pagos a sus proveedores exportando un archivo junto con la información de pago desde las líneas de diario.</span><span class="sxs-lookup"><span data-stu-id="682b4-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span></span> <span data-ttu-id="682b4-105">Después, puede cargar el archivo al banco electrónico donde procesar las transferencias de dinero relacionadas.</span><span class="sxs-lookup"><span data-stu-id="682b4-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="682b4-106"> admite el formato de transferencia de crédito SEPA, pero en su país o región, es posible que haya otros formatos para pagos electrónicos.</span><span class="sxs-lookup"><span data-stu-id="682b4-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>   

 <span data-ttu-id="682b4-107">Para habilitar las transferencias de crédito de SEPA, primero debe configurar una cuenta bancaria, un proveedor y la sección de diario general en el que se basa el diario de pagos.</span><span class="sxs-lookup"><span data-stu-id="682b4-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span></span> <span data-ttu-id="682b4-108">A continuación, prepare los pagos a los proveedores; para ello, rellene automáticamente la ventana **Diario de pagos** con los pagos por vencimientos con fechas de registro específicas.</span><span class="sxs-lookup"><span data-stu-id="682b4-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="682b4-109">Cuando haya comprobado que el banco ha procesado correctamente los pagos, puede continuar con el registro de las líneas del diario de pagos.</span><span class="sxs-lookup"><span data-stu-id="682b4-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span></span>  

 <span data-ttu-id="682b4-110">En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.</span><span class="sxs-lookup"><span data-stu-id="682b4-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="682b4-111">**Para**</span><span class="sxs-lookup"><span data-stu-id="682b4-111">**To**</span></span>|<span data-ttu-id="682b4-112">**Vea**</span><span class="sxs-lookup"><span data-stu-id="682b4-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="682b4-113">Active la función de servicio de conversión de datos bancarios para convertir los archivos de extracto de cuenta a un formato que pueda importar o para tener los archivos de pago exportados convertidos al formato que el banco requiere.</span><span class="sxs-lookup"><span data-stu-id="682b4-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span></span>|[<span data-ttu-id="682b4-114">Procedimiento: Configuración del servicio de conversión de datos bancarios</span><span class="sxs-lookup"><span data-stu-id="682b4-114">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)|  
|<span data-ttu-id="682b4-115">Configure un banco, un proveedor y un diario de pagos para la transferencia de crédito de SEPA.</span><span class="sxs-lookup"><span data-stu-id="682b4-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="682b4-116">Configuración de transferencias de crédito SEPA</span><span class="sxs-lookup"><span data-stu-id="682b4-116">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="682b4-117">Rellenar el diario de pagos con líneas de pagos vencidos a proveedores, con opción de insertar fechas de registro según la fecha de vencimiento de los documentos de compra relacionados.</span><span class="sxs-lookup"><span data-stu-id="682b4-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span></span>|[<span data-ttu-id="682b4-118">Gestionar pagos</span><span class="sxs-lookup"><span data-stu-id="682b4-118">Manage Payables</span></span>](payables-manage-payables.md)|  
|<span data-ttu-id="682b4-119">Exportar líneas de diario de pagos a un archivo en formato de transferencia de crédito SEPA.</span><span class="sxs-lookup"><span data-stu-id="682b4-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span></span>|[<span data-ttu-id="682b4-120">Exportación de pagos a un archivo de banco</span><span class="sxs-lookup"><span data-stu-id="682b4-120">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="682b4-121">Consulte los pagos que se han exportado y los archivos a los que se han exportado.</span><span class="sxs-lookup"><span data-stu-id="682b4-121">Review which payments have been exported and into which files.</span></span>|<span data-ttu-id="682b4-122">Registros de transferencia de crédito</span><span class="sxs-lookup"><span data-stu-id="682b4-122">Credit Transfer Registers</span></span>|  
|<span data-ttu-id="682b4-123">Cuando el banco procese correctamente el pago electrónico, registre los pagos.</span><span class="sxs-lookup"><span data-stu-id="682b4-123">When the electronic payment is successfully processed by the bank, post the payments.</span></span>|[<span data-ttu-id="682b4-124">Trabajar con diarios generales</span><span class="sxs-lookup"><span data-stu-id="682b4-124">Working with General Journals</span></span>](ui-work-general-journals.md)|  

## <a name="see-also"></a><span data-ttu-id="682b4-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="682b4-125">See Also</span></span>  
[<span data-ttu-id="682b4-126">Procedimiento: Configuración del servicio de conversión de datos bancarios</span><span class="sxs-lookup"><span data-stu-id="682b4-126">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)  
[<span data-ttu-id="682b4-127">Configuración de transferencias de crédito SEPA</span><span class="sxs-lookup"><span data-stu-id="682b4-127">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)  
<span data-ttu-id="682b4-128">[Gestionar pagos](payables-manage-payables.md) </span><span class="sxs-lookup"><span data-stu-id="682b4-128">[Manage Payables](payables-manage-payables.md) </span></span>  
[<span data-ttu-id="682b4-129">Trabajar con diarios generales</span><span class="sxs-lookup"><span data-stu-id="682b4-129">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="682b4-130">Cobro de pagos mediante adeudo directo SEPA</span><span class="sxs-lookup"><span data-stu-id="682b4-130">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   
