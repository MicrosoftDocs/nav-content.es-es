---
title: Crear flujos de trabajo
description: "Puede crear flujos de trabajo que vinculen tareas de procesos empresariales realizadas por distintos usuarios. Las tareas de sistema, como registros automáticos, se pueden incluir como pasos en los flujos de trabajo, antes o después de las tareas de usuario. Solicitar y conceder aprobaciones para crear registros nuevos son pasos habituales de un flujo de trabajo."
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
ms.openlocfilehash: fcf0a0c9ffc12de6fe21adb2a0906f241374aa2c
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-workflows"></a><span data-ttu-id="af219-105">Procedimiento: Crear flujos de trabajo</span><span class="sxs-lookup"><span data-stu-id="af219-105">How to: Create Workflows</span></span>
<span data-ttu-id="af219-106">Puede crear flujos de trabajo que vinculen tareas de procesos empresariales realizadas por distintos usuarios.</span><span class="sxs-lookup"><span data-stu-id="af219-106">You can create workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="af219-107">Las tareas de sistema, como registros automáticos, se pueden incluir como pasos en los flujos de trabajo, antes o después de las tareas de usuario.</span><span class="sxs-lookup"><span data-stu-id="af219-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="af219-108">Solicitar y conceder aprobaciones para crear registros nuevos son pasos habituales de un flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

<span data-ttu-id="af219-109">En la ventana **Flujo de trabajo** creas un flujo de trabajo haciendo una lista de los pasos utilizados en las líneas.</span><span class="sxs-lookup"><span data-stu-id="af219-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="af219-110">Cada paso consta de un evento del flujo de trabajo moderado por condiciones de evento y una respuesta de flujo de trabajo con opciones de respuesta.</span><span class="sxs-lookup"><span data-stu-id="af219-110">Each step consists of a workflow event moderated by event conditions and a workflow response with response options.</span></span> <span data-ttu-id="af219-111">Los pasos del flujo de trabajo se definen rellenando los campos de las líneas de flujo de trabajo en listas fijas de valores de evento y respuesta que representan los escenarios de flujo de trabajo que admite el código de aplicación.</span><span class="sxs-lookup"><span data-stu-id="af219-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

<span data-ttu-id="af219-112">Al crear flujos de trabajo, puede copiar los pasos de flujos de trabajo existentes o de plantillas de flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-112">When you create workflows, you can copy the steps from existing workflows or from workflow templates.</span></span> <span data-ttu-id="af219-113">Las plantillas de flujo de trabajo representan flujos de trabajo no editables que existen en la versión genérica de [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="af219-113">Workflow templates represent non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="af219-114">El código de las plantillas de flujo de trabajo agregados por Microsoft se prefija con “MS-“, como “MS-PIW”.</span><span class="sxs-lookup"><span data-stu-id="af219-114">The code for workflow templates that are added by Microsoft are prefixed with “MS-“, such as in “MS-PIW”.</span></span> <span data-ttu-id="af219-115">Para obtener más información, consulte [Procedimiento: crear flujos de trabajo a partir de plantillas de flujo de trabajo](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="af219-115">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

<span data-ttu-id="af219-116">Si su escenario empresarial necesita eventos de flujo de trabajo o respuestas que no se admiten, un asociado de Microsoft debe implementarlos personalizando el código de aplicación.</span><span class="sxs-lookup"><span data-stu-id="af219-116">If your business scenario requires workflow events or responses that are not supported, a Microsoft partner must implement them by customizing the application code.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="af219-117">Todas las notificaciones sobre pasos de flujo de trabajo se envían a través de una cola de proyectos.</span><span class="sxs-lookup"><span data-stu-id="af219-117">All notifications about workflow steps are sent through a job queue.</span></span> <span data-ttu-id="af219-118">Asegúrese de que la cola de proyectos en la instalación está configurada para gestionar las notificaciones de flujo de trabajo, así como que la casilla **Iniciar automáticamente desde NAS** esté seleccionada.</span><span class="sxs-lookup"><span data-stu-id="af219-118">Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From NAS** check box is selected.</span></span> <span data-ttu-id="af219-119">Para obtener más información, consulte [Uso de colas de proyectos para programar tareas](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="af219-119">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>  

## <a name="to-create-a-workflow"></a><span data-ttu-id="af219-120">Para crear un flujo de trabajo</span><span class="sxs-lookup"><span data-stu-id="af219-120">To create a workflow</span></span>  
1. <span data-ttu-id="af219-121">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Flujos de trabajo** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="af219-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af219-122">Seleccione la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="af219-122">Choose the **New** action.</span></span> <span data-ttu-id="af219-123">Se abre la ventana **Flujo de trabajo**.</span><span class="sxs-lookup"><span data-stu-id="af219-123">The **Workflow** window opens.</span></span>  
3. <span data-ttu-id="af219-124">En el campo **Código**, introduzca un máximo de 20 caracteres para identificar el flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-124">In the **Code** field, enter a maximum of 20 characters to identify the workflow.</span></span>  
4. <span data-ttu-id="af219-125">Para crear el flujo de trabajo desde una plantilla, en la ventana **Flujos de trabajo**, seleccione la acción **Crear flujo de trabajo desde plantilla**.</span><span class="sxs-lookup"><span data-stu-id="af219-125">To create the workflow from a workflow template, in the **Workflows** window, choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="af219-126">Para obtener más información, consulte [Procedimiento: crear flujos de trabajo a partir de plantillas de flujo de trabajo](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="af219-126">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  
5. <span data-ttu-id="af219-127">En el campo **Descripción**, describa el flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-127">In the **Description** field, describe the workflow.</span></span>  
6. <span data-ttu-id="af219-128">En el campo **Categoría**, especifique a qué categoría pertenece el flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-128">In the **Category** field, specify which category the workflow belongs to.</span></span>  
7. <span data-ttu-id="af219-129">En el campo **Evento Cuando**, especifique el evento que debe producirse para iniciar el paso del flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-129">In the **When Event** field, specify the event that must occur to start the workflow step.</span></span>  

    <span data-ttu-id="af219-130">Cuando elige el campo, la ventana **Eventos de flujo de trabajo** se abre, donde puede seleccionar de todos los eventos de flujo de trabajo existentes.</span><span class="sxs-lookup"><span data-stu-id="af219-130">When you choose the field, the **Workflow Events** window opens where you select from all the workflow events that exist.</span></span>  
8. <span data-ttu-id="af219-131">En el campo **Condición**, especifique una o varias condiciones que se deben cumplir para que se produzca el evento en el campo **Evento Cuando**.</span><span class="sxs-lookup"><span data-stu-id="af219-131">In the **Condition** field, specify one or more conditions that must be met before the event in the **When Event** field can occur.</span></span>  

    <span data-ttu-id="af219-132">Cuando elige el campo se abre la ventana **Condiciones de evento**, donde se elige entre una lista de campos de filtro pertinentes relevantes como condiciones del evento en cuestión.</span><span class="sxs-lookup"><span data-stu-id="af219-132">When you choose the field, the **Event Conditions** window opens where you choose from a list of filter fields that are relevant as conditions for the event in question.</span></span> <span data-ttu-id="af219-133">Puede agregar los campos de filtro nuevos que desee utilizar como condiciones del evento.</span><span class="sxs-lookup"><span data-stu-id="af219-133">You can add new filter fields that you want to use as event conditions.</span></span> <span data-ttu-id="af219-134">Puede definir filtros de condición de evento igual que define filtros en las páginas de solicitud de informe.</span><span class="sxs-lookup"><span data-stu-id="af219-134">You set event condition filters just as you set filters on report request pages.</span></span>  

    <span data-ttu-id="af219-135">Si el evento del flujo de trabajo es el cambio de un campo determinado en un registro, la ventana **Condiciones del evento** se abre con las opciones para seleccionar el campo y el tipo de cambio.</span><span class="sxs-lookup"><span data-stu-id="af219-135">If the workflow event is the change of a specific field on a record, then the **Event Conditions** window opens with options to select the field and the type of change.</span></span>  

    1.  <span data-ttu-id="af219-136">Para especificar un cambio de campo para el evento, en la ventana **Condiciones del evento**, en el campo **Campo**, seleccione el campo que cambia.</span><span class="sxs-lookup"><span data-stu-id="af219-136">To specify a field change for the event, in the **Event Conditions** window, in the **Field** field, select the field that changes.</span></span>  
    2.  <span data-ttu-id="af219-137">En el campo **Operador**, seleccione **Disminuyó**, **Aumentó** o **Cambió**.</span><span class="sxs-lookup"><span data-stu-id="af219-137">In the **Operator** field, select either **Decreased**, **Increased**, or **Changed**.</span></span>  
9. <span data-ttu-id="af219-138">Especifique la respuesta que seguirá cuando se produzca el evento del flujo de trabajo en el campo **Respuesta Entonces**.</span><span class="sxs-lookup"><span data-stu-id="af219-138">In the **Then Response** field, specify the response that will follow when the workflow event occurs.</span></span>  

     <span data-ttu-id="af219-139">Cuando elija el campo, la ventana **Respuestas de flujo de trabajo** se abre, donde puede seleccionar de todas las respuestas de flujo de trabajo que existen y fijar opciones de respuesta para la respuesta seleccionada.</span><span class="sxs-lookup"><span data-stu-id="af219-139">When you choose the field, the **Workflow Responses** window opens where you select from all workflow responses that exist and set response options for the selected response.</span></span>  
10. <span data-ttu-id="af219-140">En la ficha desplegable **Opciones para la respuesta seleccionada**, especifique las opciones para la respuesta de flujo de trabajo seleccionando los valores en los campos que aparecen, como se indica a continuación:</span><span class="sxs-lookup"><span data-stu-id="af219-140">On the **Options for the Selected Response** FastTab, specify options for the workflow response, by selecting values in the different fields that appear, as follows:</span></span>  

    1.  <span data-ttu-id="af219-141">Para especificar las opciones para una respuesta de flujo de trabajo que implica enviar una notificación, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="af219-141">To specify options for a workflow response that involves sending a notification, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="af219-142">Campo</span><span class="sxs-lookup"><span data-stu-id="af219-142">Field</span></span>|<span data-ttu-id="af219-143">Description</span><span class="sxs-lookup"><span data-stu-id="af219-143">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="af219-144">**Id. de usuario destinatario**</span><span class="sxs-lookup"><span data-stu-id="af219-144">**Recipient User ID**</span></span>|<span data-ttu-id="af219-145">Especifique el usuario al que se debe enviar la notificación.</span><span class="sxs-lookup"><span data-stu-id="af219-145">Specify the user who the notification must be sent to.</span></span> <span data-ttu-id="af219-146">Nota: Esta opción solo está disponible para respuestas de flujo de trabajo con un marcador para un usuario específico.</span><span class="sxs-lookup"><span data-stu-id="af219-146">Note: This option is only available for workflow responses with a placeholder for a specific user.</span></span> <span data-ttu-id="af219-147">Para las respuestas de flujo de trabajo sin marcadores para usuarios, el usuario de aprobación define normalmente la configuración del destinatario de la notificación.</span><span class="sxs-lookup"><span data-stu-id="af219-147">For workflow responses without placeholders for users, the notification recipient is typically defined by the approval user setup.</span></span>|  
        |<span data-ttu-id="af219-148">**Página de destino de vínculo**</span><span class="sxs-lookup"><span data-stu-id="af219-148">**Link Target Page**</span></span>|<span data-ttu-id="af219-149">Especifique otra página en [!INCLUDE[d365fin](includes/d365fin_md.md)] que el vínculo de la notificación abrirá en lugar de la página predeterminada.</span><span class="sxs-lookup"><span data-stu-id="af219-149">Specify another page in [!INCLUDE[d365fin](includes/d365fin_md.md)] that the link in the notification opens instead of the default page.</span></span>|  
        |<span data-ttu-id="af219-150">**Personalizar vínculo**</span><span class="sxs-lookup"><span data-stu-id="af219-150">**Custom Link**</span></span>|<span data-ttu-id="af219-151">Especifique la dirección URL de un vínculo que se agrega a la notificación además del vínculo a la página en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="af219-151">Specify the URL of a link that is added to the notification in addition to the link to page in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|  
    2.  <span data-ttu-id="af219-152">Para especificar opciones para una respuesta de flujo de trabajo que implica crear una solicitud de aprobación, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="af219-152">To specify options for a workflow response that involves creating an approval request, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="af219-153">Campo</span><span class="sxs-lookup"><span data-stu-id="af219-153">Field</span></span>|<span data-ttu-id="af219-154">Description</span><span class="sxs-lookup"><span data-stu-id="af219-154">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="af219-155">**Fórmula fecha vencimiento**</span><span class="sxs-lookup"><span data-stu-id="af219-155">**Due Date Formula**</span></span>|<span data-ttu-id="af219-156">Especifique la cantidad de días en que se debe completar la solicitud de aprobación desde la fecha en que se ha enviado.</span><span class="sxs-lookup"><span data-stu-id="af219-156">Specify in how many days the approval request must be resolved from the date when it was sent.</span></span>|  
        |<span data-ttu-id="af219-157">**Delegar tras**</span><span class="sxs-lookup"><span data-stu-id="af219-157">**Delegate After**</span></span>|<span data-ttu-id="af219-158">Especifica si y cuándo se delegará automáticamente una solicitud de aprobación al sustituto correspondiente.</span><span class="sxs-lookup"><span data-stu-id="af219-158">Specify if and when an approval request will automatically be delegated to the relevant substitute.</span></span> <span data-ttu-id="af219-159">Puede seleccionar delegar automáticamente un día, dos o cinco después de la fecha en que se solicitó la aprobación.</span><span class="sxs-lookup"><span data-stu-id="af219-159">You can select to automatically delegate one, two, or five days after the date when the approval was requested.</span></span>|  
        |<span data-ttu-id="af219-160">**Tipo de aprobador**</span><span class="sxs-lookup"><span data-stu-id="af219-160">**Approver Type**</span></span>|<span data-ttu-id="af219-161">Especifique quién es el aprobador según la configuración de usuarios de aprobación y usuarios de flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-161">Specify who the approver is, according to the setup of approval users and workflow users.</span></span><br /><br /> <span data-ttu-id="af219-162">Las siguientes opciones están disponibles:</span><span class="sxs-lookup"><span data-stu-id="af219-162">The following options exist:</span></span><br /><br /> <span data-ttu-id="af219-163">-   **Vendedor/Comprador** especifica que el usuario configurado en el campo **Cód. vendedor/comprador** en la ventana **Config. usuario aprobación** determina quién es el aprobador.</span><span class="sxs-lookup"><span data-stu-id="af219-163">-   **Salesperson/Purchaser** specifies that the user who is set up in the **Salespers./Purch. Code** field in the **Approval User Setup** window determines the approver.</span></span> <span data-ttu-id="af219-164">Los movimientos de solicitud de aprobación se crean según el valor del campo **Tipo de límite de aprobador**.</span><span class="sxs-lookup"><span data-stu-id="af219-164">Approval request entries are then created according to the value in the **Approver Limit Type** field.</span></span><br />     <span data-ttu-id="af219-165">Para obtener más información, vea [Procedimiento: Configurar usuarios de aprobación](across-how-to-set-up-workflow-users.md).</span><span class="sxs-lookup"><span data-stu-id="af219-165">For more information, see [How to: Set Up Approval Users](across-how-to-set-up-workflow-users.md).</span></span>|  
        |<span data-ttu-id="af219-166">**Mostrar mensaje de confirmación**</span><span class="sxs-lookup"><span data-stu-id="af219-166">**Show Confirmation Message**</span></span>|<span data-ttu-id="af219-167">Especifica si un mensaje de confirmación se muestra los usuarios después de que hayan solicitado una aprobación.</span><span class="sxs-lookup"><span data-stu-id="af219-167">Specify if a confirmation message is shown to users after they request an approval.</span></span>|  
        |<span data-ttu-id="af219-168">**Tipo de límite de aprobador**</span><span class="sxs-lookup"><span data-stu-id="af219-168">**Approver Limit Type**</span></span>|<span data-ttu-id="af219-169">Especifique cómo afectan los límites de aprobación de los aprobadores cuando se crean movimientos de solicitud de aprobación para ellos.</span><span class="sxs-lookup"><span data-stu-id="af219-169">Specify how approvers’ approval limits affect when approval request entries are created for them.</span></span> <span data-ttu-id="af219-170">Un aprobador calificado es aquel cuyo límite de aprobación es superior al valor de la solicitud que se está realizando.</span><span class="sxs-lookup"><span data-stu-id="af219-170">A qualified approver is an approver whose approval limit is above the value on the request being made.</span></span><br /><br /> <span data-ttu-id="af219-171">Las siguientes opciones están disponibles:</span><span class="sxs-lookup"><span data-stu-id="af219-171">The following options exist:</span></span><br /><br /> <span data-ttu-id="af219-172">1.  **Cadena de aprobadores** especifica que los movimientos de solicitud de aprobación se crean para todos los aprobadores del solicitante hasta el primer aprobador cualificado, incluido este.</span><span class="sxs-lookup"><span data-stu-id="af219-172">1.  **Approver Chain** specifies that approval request entries are created for all the requester’s approvers up to and including the first qualified approver.</span></span><br /><span data-ttu-id="af219-173">2.  **Aprobador directo** especifica que un movimiento de solicitud de aprobación solo se crea para el aprobador inmediato del solicitante, sea cual sea el límite de aprobación del aprobador.</span><span class="sxs-lookup"><span data-stu-id="af219-173">2.  **Direct Approver** specifies that an approval request entry is only created for the requester’s immediate approver, regardless of the approver’s approval limit.</span></span><br /><span data-ttu-id="af219-174">3.  **Primer aprobador cualificado** especifica que solo se crea un movimiento de solicitud de aprobación para el primer aprobador cualificado del solicitante.</span><span class="sxs-lookup"><span data-stu-id="af219-174">3.  **First Qualified Approver** specifies that an approval request entry is only created for the requester’s first qualified approver.</span></span><br />|  
    3.  <span data-ttu-id="af219-175">Para especificar las opciones para una respuesta de flujo de trabajo que implica crear líneas de diario, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="af219-175">To specify options for a workflow response that involves creating journal lines, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="af219-176">Campo</span><span class="sxs-lookup"><span data-stu-id="af219-176">Field</span></span>|<span data-ttu-id="af219-177">Description</span><span class="sxs-lookup"><span data-stu-id="af219-177">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="af219-178">**Nombre plantilla diario general**</span><span class="sxs-lookup"><span data-stu-id="af219-178">**General Journal Template Name**</span></span>|<span data-ttu-id="af219-179">Especifique el nombre de la plantilla de libro de diario general en las que se crearán las líneas de diario especificadas.</span><span class="sxs-lookup"><span data-stu-id="af219-179">Specify the name of the general journal template that the specified journal lines are created in.</span></span>|  
        |<span data-ttu-id="af219-180">**Nombre sección diario general**</span><span class="sxs-lookup"><span data-stu-id="af219-180">**General Journal Batch Name**</span></span>|<span data-ttu-id="af219-181">Especifique el nombre del proceso de diario general en las que se crearán las líneas de diario especificadas.</span><span class="sxs-lookup"><span data-stu-id="af219-181">Specify the name of the general journal batch that the specified journal lines are created in.</span></span>|  

11. <span data-ttu-id="af219-182">Seleccione los botones **Aumentar sangría** y **Disminuir sangría** para sangrar el nombre del evento en el campo **Cuando** para definir la posición del paso de flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="af219-182">Choose the **Increase Indent** and **Decrease Indent** buttons to indent the event name in the **When** field to define the step’s position in the workflow.</span></span>  
    1.  <span data-ttu-id="af219-183">Indique que el paso es el siguiente de la secuencia del flujo de trabajo aplicando sangría en el nombre del evento del evento del paso anterior.</span><span class="sxs-lookup"><span data-stu-id="af219-183">Indicate that the step is the next in the workflow sequence by indenting the event name under the event name of the previous step.</span></span>  
    2.  <span data-ttu-id="af219-184">Indique que el paso es uno de más pasos alternativos que pueden iniciarse en función de la condición colocando el nombre del evento en el mismo sangrado que los otros pasos alternativos.</span><span class="sxs-lookup"><span data-stu-id="af219-184">Indicate that the step is one of more alternative steps that may start depending on its condition by placing the event name at the same indentation as the other alternative steps.</span></span> <span data-ttu-id="af219-185">Ordene estos pasos opcionales según la prioridad colocando el paso más importante primero.</span><span class="sxs-lookup"><span data-stu-id="af219-185">Order such optional steps according to priority by placing the most important step first.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="af219-186">Puede cambiar solo la sangría de un paso que no tenga un paso subsiguiente.</span><span class="sxs-lookup"><span data-stu-id="af219-186">You can only change the indent of a step that does not have a subsequent step.</span></span>  

12. <span data-ttu-id="af219-187">Repita los pasos del 7 al 11 para añadir más pasos de flujo de trabajo antes o después del paso que acaba de crear.</span><span class="sxs-lookup"><span data-stu-id="af219-187">Repeat steps 7 through 11 to add more workflow steps, either before or after the step that you have just created.</span></span>  
13. <span data-ttu-id="af219-188">Seleccione la casilla **Habilitado** para especificar que el flujo de trabajo empezará en cuanto se produzca el evento en el primer paso de tipo **Punto de entrada**.</span><span class="sxs-lookup"><span data-stu-id="af219-188">Select the **Enabled** check box to specify that the workflow will start as soon as the event on the first step of type **Entry Point** occurs.</span></span> <span data-ttu-id="af219-189">Para obtener más información, consulte [Uso de flujos de trabajo](across-use-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="af219-189">For more information, see [Using Workflows](across-use-workflows.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="af219-190">No habilite un flujo de trabajo hasta que esté seguro de que el flujo de trabajo esté completado y que los pasos del flujo de trabajo relacionado puedan comenzar.</span><span class="sxs-lookup"><span data-stu-id="af219-190">Do not enable a workflow until you are sure that the workflow is completed and that the involved workflow steps can start.</span></span>  

> [!TIP]  
>  <span data-ttu-id="af219-191">Para ver las relaciones entre las tablas que se utilizan en los flujos de trabajo, seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe") y, a continuación, introduzca **Flujo de trabajo: relaciones de tabla**.</span><span class="sxs-lookup"><span data-stu-id="af219-191">To see relations between tables that are used in workflows, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and then enter **Workflow – Table Relations**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="af219-192">Consulte también</span><span class="sxs-lookup"><span data-stu-id="af219-192">See Also</span></span>  
<span data-ttu-id="af219-193">[Procedimiento: crear flujos de trabajo a partir de plantillas de flujo de trabajo](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="af219-193">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
<span data-ttu-id="af219-194">[Procedimiento: Configurar usuarios de aprobación](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="af219-194">[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
<span data-ttu-id="af219-195">[Configurar notificaciones de flujo de trabajo](across-setting-up-workflow-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="af219-195">[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md) </span></span>  
<span data-ttu-id="af219-196">[Procedimiento: Ver las instancias de paso de flujo de trabajo archivadas](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="af219-196">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
<span data-ttu-id="af219-197">[Procedimiento: Eliminar flujos de trabajo](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="af219-197">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
<span data-ttu-id="af219-198">[Tutorial: Configuración y uso de un flujo de trabajo de aprobación de compra](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="af219-198">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
<span data-ttu-id="af219-199">[Configuración de flujos de trabajo](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="af219-199">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
<span data-ttu-id="af219-200">[Uso de flujos de trabajo](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="af219-200">[Using Workflows](across-use-workflows.md) </span></span>  
[<span data-ttu-id="af219-201">Flujo de trabajo</span><span class="sxs-lookup"><span data-stu-id="af219-201">Workflow</span></span>](across-workflow.md)      

