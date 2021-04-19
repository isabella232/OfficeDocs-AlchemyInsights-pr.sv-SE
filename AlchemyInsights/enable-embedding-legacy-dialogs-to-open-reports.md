---
title: Aktivera inbäddning av äldre dialogrutor för att öppna rapporter
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814282"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c80c5-102">Aktivera inbäddning av äldre dialogrutor för att öppna rapporter</span><span class="sxs-lookup"><span data-stu-id="c80c5-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c80c5-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="c80c5-103">**Symptom**</span></span>

<span data-ttu-id="c80c5-104">Användare kan inte öppna rapporter.</span><span class="sxs-lookup"><span data-stu-id="c80c5-104">Users are unable to open reports.</span></span> <span data-ttu-id="c80c5-105">"Något gick fel.</span><span class="sxs-lookup"><span data-stu-id="c80c5-105">"Something has gone wrong.</span></span> <span data-ttu-id="c80c5-106">Mer information finns i den tekniska informationen."</span><span class="sxs-lookup"><span data-stu-id="c80c5-106">Check technical details for more details."</span></span>

<span data-ttu-id="c80c5-107">**Orsak**</span><span class="sxs-lookup"><span data-stu-id="c80c5-107">**Cause**</span></span>

<span data-ttu-id="c80c5-108">Rapporter kan inte läsas in i UCI med felet, "Formulärbeskrivning är null eller inte definierat".</span><span class="sxs-lookup"><span data-stu-id="c80c5-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c80c5-109">Rapporter i UCI kräver fortfarande äldre dialogrutor, så kundens system måste ha *tillåts förlegacydialogsembedding* aktiverat.</span><span class="sxs-lookup"><span data-stu-id="c80c5-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c80c5-110">**Lösning**</span><span class="sxs-lookup"><span data-stu-id="c80c5-110">**Solution**</span></span>

1. <span data-ttu-id="c80c5-111">Gå till **Inställningar >Administration > Systeminställningar > Fliken Allmänt.**</span><span class="sxs-lookup"><span data-stu-id="c80c5-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c80c5-112">Ställ in "Aktivera inbäddning av vissa äldre dialogrutor i Unified Interface-webbläsarklienten" till **Ja.**</span><span class="sxs-lookup"><span data-stu-id="c80c5-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
