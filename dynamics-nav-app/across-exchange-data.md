---
title: Intercambio de datos
description: "Puede intercambiar datos entre [!INCLUDE[d365fin](includes/d365fin_md.md)] y secuencias o archivos externos en conexión con tareas de negocio comunes, como enviar y recibir documentos electrónicos e importar y exportar archivos bancarios."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e41e0eb6dd10127a47b2b6545d0333db700586bc
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="exchanging-data"></a><span data-ttu-id="c393a-103">Intercambio de datos</span><span class="sxs-lookup"><span data-stu-id="c393a-103">Exchanging Data</span></span>
<span data-ttu-id="c393a-104">Puede intercambiar datos entre [!INCLUDE[d365fin](includes/d365fin_md.md)] y secuencias o archivos externos en conexión con tareas de negocio comunes, como enviar y recibir documentos electrónicos e importar y exportar archivos bancarios.</span><span class="sxs-lookup"><span data-stu-id="c393a-104">You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.</span></span>  

<span data-ttu-id="c393a-105">Para poder enviar y recibir documentos electrónicos o importar y exportar archivos bancarios, debe configurar el marco de intercambio de datos para procesar las secuencias o los archivos de datos correspondientes.</span><span class="sxs-lookup"><span data-stu-id="c393a-105">Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved data files or streams.</span></span> <span data-ttu-id="c393a-106">Además, debe configurar áreas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="c393a-106">In addition, you must set up related areas.</span></span> <span data-ttu-id="c393a-107">Estos incluyen los datos maestros para los clientes a los que envían las facturas electrónicas y el servicio de la conversión de datos bancarios en los casos en que distribuya conversiones de archivos bancarios a un proveedor de servicios externo.</span><span class="sxs-lookup"><span data-stu-id="c393a-107">These include master data for customers that you send electronic invoices to and the bank data conversion service in case you distribute bank file conversions to an external service provider.</span></span> <span data-ttu-id="c393a-108">Para obtener más información, consulte [Configurar el intercambio de datos](across-set-up-data-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="c393a-108">For more information, see [Setting Up Data Exchange](across-set-up-data-exchange.md).</span></span>  

 <span data-ttu-id="c393a-109">En la tabla siguiente se indican una serie de tareas con vínculos a los temas que las describen.</span><span class="sxs-lookup"><span data-stu-id="c393a-109">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="c393a-110">**Para**</span><span class="sxs-lookup"><span data-stu-id="c393a-110">**To**</span></span>|<span data-ttu-id="c393a-111">**Consulte**</span><span class="sxs-lookup"><span data-stu-id="c393a-111">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="c393a-112">Convertir registros de documentos de venta en [!INCLUDE[d365fin](includes/d365fin_md.md)] a un formato estándar y enviarlos como documentos electrónicos que los clientes pueden recibir en su sistema.</span><span class="sxs-lookup"><span data-stu-id="c393a-112">Convert sales document records in [!INCLUDE[d365fin](includes/d365fin_md.md)] to a standardized format and send them as electronic documents that your customers can receive into their system.</span></span>|[<span data-ttu-id="c393a-113">Procedimiento: Enviar documentos electrónicos</span><span class="sxs-lookup"><span data-stu-id="c393a-113">How to: Send Electronic Documents</span></span>](sales-how-to-send-electronic-documents.md)|  
|<span data-ttu-id="c393a-114">Enviar un PDF o archivos de imagen a un proveedor de servicios de OCR y recibirlos como documentos electrónicos que se pueden convertir a registros de documento en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c393a-114">Send PDF or image files to a provider of OCR services, and receive them back as electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="c393a-115">Utilizar el servicio OCR para convertir archivos PDF y de imagen en documentos electrónicos</span><span class="sxs-lookup"><span data-stu-id="c393a-115">How to: Use OCR to Turn PDF and Image Files into Electronic Documents</span></span>](across-how-use-ocr-pdf-images-files.md)|  
|<span data-ttu-id="c393a-116">Recibir documentos electrónicos, del servicio OCR o del servicio de intercambio de documentos, en un formato estándar que usted convertirá a los registros de documento relevantes en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c393a-116">Receive electronic documents, either from the OCR service or the document exchange service, in a standardized format that you convert to the relevant document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="c393a-117">Procedimiento: recibir y convertir documentos electrónicos</span><span class="sxs-lookup"><span data-stu-id="c393a-117">How to: Receive and Convert Electronic Documents</span></span>](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|<span data-ttu-id="c393a-118">Importe un archivo de extracto bancario a la ventana **Diario de conciliación de pagos** como el primer paso para conciliar pagos o a la ventana **Conciliación banco** como el primer paso para conciliar cuentas bancarias.</span><span class="sxs-lookup"><span data-stu-id="c393a-118">Import a bank statement file into the **Payment Reconciliation Journal** window as the first step in reconciling payments or into the **Bank Acc. Reconciliation** window as the first step in reconciling bank accounts.</span></span>|<span data-ttu-id="c393a-119">[Liquidar pagos automáticamente y conciliar cuentas bancarias][Liquidar pagos automáticamente y conciliar cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="c393a-119">[Apply Payments Automatically and Reconcile Bank Accounts]([Applying Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md)</span></span>|  
|<span data-ttu-id="c393a-120">Exportar pagos desde la ventana **Diario de pagos** a un archivo bancario que se cargará en la cuenta bancaria electrónica para su procesamiento.</span><span class="sxs-lookup"><span data-stu-id="c393a-120">Export payments from the **Payment Journal** window to a bank file that you upload to your electronic bank account for processing.</span></span>|[<span data-ttu-id="c393a-121">Exportación de pagos a un archivo de banco</span><span class="sxs-lookup"><span data-stu-id="c393a-121">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="c393a-122">Indique a su banco para que transfiera los importes de pago de los bancos de los clientes a la cuenta de su empresa según la configuración de adeudo directo SEPA.</span><span class="sxs-lookup"><span data-stu-id="c393a-122">Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.</span></span>|[<span data-ttu-id="c393a-123">Creación de movimientos de domiciliación de adeudo directo SEPA y exportación a un archivo bancario</span><span class="sxs-lookup"><span data-stu-id="c393a-123">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|<span data-ttu-id="c393a-124">Utilice un proveedor de servicios de tipos de cambio de divisa para actualizar la ventana **Divisas**.</span><span class="sxs-lookup"><span data-stu-id="c393a-124">Use a service provider of currency exchange rates to update the **Currencies** window.</span></span>|[<span data-ttu-id="c393a-125">Actualizar los tipos de cambio de divisa</span><span class="sxs-lookup"><span data-stu-id="c393a-125">How to: Update Currency Exchange Rates</span></span>](finance-how-update-currencies.md)|  
|<span data-ttu-id="c393a-126">Ver qué elementos de archivo están asignados a campos de [!INCLUDE[d365fin](includes/d365fin_md.md)] al importar archivos de extracto CAMT de SEPA.</span><span class="sxs-lookup"><span data-stu-id="c393a-126">View which file elements are mapped to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] when importing SEPA CAMT statement files.</span></span>|[<span data-ttu-id="c393a-127">Asignación de campos al importar archivos CAMT de SEPA</span><span class="sxs-lookup"><span data-stu-id="c393a-127">Field Mapping When Importing SEPA CAMT Files</span></span>](across-field-mapping-when-importing-sepa-camt-files.md)|  
|<span data-ttu-id="c393a-128">Ver qué campos de [!INCLUDE[d365fin](includes/d365fin_md.md)] están asignados a elementos de archivo al exportar archivos de pago con la función de servicio de conversión de datos bancarios.</span><span class="sxs-lookup"><span data-stu-id="c393a-128">View which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to file elements when exporting payment files by using the Bank Date Conversion Service feature.</span></span>|[<span data-ttu-id="c393a-129">Asignación de campos al exportar archivos de pago con el servicio de conversión de datos bancarios</span><span class="sxs-lookup"><span data-stu-id="c393a-129">Field Mapping When Exporting Payment Files Using Bank Data Conversion Service</span></span>](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a><span data-ttu-id="c393a-130">Consulte también</span><span class="sxs-lookup"><span data-stu-id="c393a-130">See Also</span></span>  
[<span data-ttu-id="c393a-131">Configuración del intercambio de datos</span><span class="sxs-lookup"><span data-stu-id="c393a-131">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="c393a-132">Intercambio de datos electrónicamente</span><span class="sxs-lookup"><span data-stu-id="c393a-132">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="c393a-133">[Facturación de ventas](sales-how-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="c393a-133">[How to: Invoice Sales](sales-how-invoice-sales.md) </span></span>  
[<span data-ttu-id="c393a-134">Procedimiento: Registro de compras</span><span class="sxs-lookup"><span data-stu-id="c393a-134">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="c393a-135">Documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="c393a-135">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="c393a-136">Funciones empresariales generales</span><span class="sxs-lookup"><span data-stu-id="c393a-136">General Business Functionality</span></span>](ui-across-business-areas.md)  
