---
title: "Configuración de rangos de fechas en Dynamics NAV"
description: "Obtenga información sobre cómo obtener un informe para mostrar datos de periodos de tiempo específicos mediante rangos de fechas en Dynamics NAV."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 05/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2619095e8b9e48068aa9d8790a9699b4c7ff05ec
ms.contentlocale: es-es
ms.lasthandoff: 10/16/2017

---
# <a name="entering-date-ranges-in-dynamics-nav"></a><span data-ttu-id="3ed1b-103">Introducir rangos de fechas en Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="3ed1b-103">Entering Date Ranges in Dynamics NAV</span></span>
<span data-ttu-id="3ed1b-104">Puede establecer filtros que contienen una fecha de inicio y de finalización para mostrar sólo los datos que se incluyen dentro de dicho rango de fechas o intervalo de tiempo.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="3ed1b-105">Se aplican reglas especiales a la forma de establecer los rangos de fechas.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="3ed1b-106">Tomemos la lista **Los 10 mejores clientes** como ejemplo:</span><span class="sxs-lookup"><span data-stu-id="3ed1b-106">Let's take the **Customer Top 10** as an example:</span></span>

![Configurar un rango de fechas en la página de solicitud de la lista de los 10 mejores clientes](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="3ed1b-108">Aquí puede limitar el informe a un rango de fechas como las últimas 2 semanas, o un total de 6 semanas, o el rango que desee.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="3ed1b-109">Para establecer los rangos de fechas, introduzca las fechas y utilice **..**</span><span class="sxs-lookup"><span data-stu-id="3ed1b-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="3ed1b-110">o **|** para definir el rango.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-110">or **|** to set the range.</span></span> <span data-ttu-id="3ed1b-111">En nuestro ejemplo, para mostrar los 10 mejores clientes de las dos primeras semanas de mayo, definiría el filtro de fecha *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="3ed1b-112">A continuación le mostramos dos ejemplos más:</span><span class="sxs-lookup"><span data-stu-id="3ed1b-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="3ed1b-113">Significado</span><span class="sxs-lookup"><span data-stu-id="3ed1b-113">Meaning</span></span> | <span data-ttu-id="3ed1b-114">Ejemplo</span><span class="sxs-lookup"><span data-stu-id="3ed1b-114">Example</span></span> | <span data-ttu-id="3ed1b-115">Movimientos incluidos</span><span class="sxs-lookup"><span data-stu-id="3ed1b-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="3ed1b-116">Igual a</span><span class="sxs-lookup"><span data-stu-id="3ed1b-116">Equal to</span></span>| <span data-ttu-id="3ed1b-117">15 12 16</span><span class="sxs-lookup"><span data-stu-id="3ed1b-117">12 15 16</span></span> |<span data-ttu-id="3ed1b-118">Solo los movimientos registrados el 15 de diciembre de 2016.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="3ed1b-119">Intervalo</span><span class="sxs-lookup"><span data-stu-id="3ed1b-119">Interval</span></span>| <span data-ttu-id="3ed1b-120">15 12 16..15 17 17</span><span class="sxs-lookup"><span data-stu-id="3ed1b-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="3ed1b-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="3ed1b-121">..12 15 16</span></span>|<span data-ttu-id="3ed1b-122">Registrados entre el 15 de diciembre de 2016 y el 15 de enero de 2017, ambos incluidos.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="3ed1b-123">Registrados el 15 de diciembre de 2016 o antes.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="3ed1b-124">O</span><span class="sxs-lookup"><span data-stu-id="3ed1b-124">Either/or</span></span>|<span data-ttu-id="3ed1b-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="3ed1b-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="3ed1b-126">Registrados el 15 de diciembre o el 16 de diciembre de 2016.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="3ed1b-127">Si hay movimientos registrados en los dos días, se mostrarán todos.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="3ed1b-128">También puede combinar los distintos tipos de formato.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="3ed1b-129">Ejemplo</span><span class="sxs-lookup"><span data-stu-id="3ed1b-129">Example</span></span> | <span data-ttu-id="3ed1b-130">Movimientos incluidos</span><span class="sxs-lookup"><span data-stu-id="3ed1b-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="3ed1b-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="3ed1b-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="3ed1b-132">Movimientos registrados el 15 de diciembre de 2016, o entre el 01 de diciembre de 2016 y el 31 de mayo de 2017, ambos incluidos.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="3ed1b-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="3ed1b-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="3ed1b-134">Los movimientos registrados el 14 de diciembre o con anterioridad, o bien los movimientos registrados el 30 de diciembre o posteriormente, es decir, todos los movimientos excepto los registrados en las fechas comprendidas entre el 15 y el 29 de diciembre, ambas inclusive.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="3ed1b-135">Observe que hemos utilizado el formato de fecha MMDDAA de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="3ed1b-136">A medida que [!INCLUDE[d365fin](includes/d365fin_md.md)] esté disponible en otros mercados, podrá utilizar los formatos a los que está acostumbrado.</span><span class="sxs-lookup"><span data-stu-id="3ed1b-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="3ed1b-137">Consulte también</span><span class="sxs-lookup"><span data-stu-id="3ed1b-137">See Also</span></span>
<span data-ttu-id="3ed1b-138">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3ed1b-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="3ed1b-139">Introducir criterios en los filtros</span><span class="sxs-lookup"><span data-stu-id="3ed1b-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="3ed1b-140">Funciones empresariales generales</span><span class="sxs-lookup"><span data-stu-id="3ed1b-140">General Business Functionality</span></span>](ui-across-business-areas.md)
