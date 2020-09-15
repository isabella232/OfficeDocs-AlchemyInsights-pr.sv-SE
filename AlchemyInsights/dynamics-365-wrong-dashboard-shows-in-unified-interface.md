---
title: Dynamics 365 – fel instrument panel visas i Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711293"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="57f6e-102">Fel instrument paneler i det enhetliga gränssnittet för Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="57f6e-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="57f6e-103">Det finns flera orsaker till att du kan se en annan instrument panel än den du förväntar dig:</span><span class="sxs-lookup"><span data-stu-id="57f6e-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="57f6e-104">Användaren har ställt in en standard instrument panel för användare</span><span class="sxs-lookup"><span data-stu-id="57f6e-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="57f6e-105">Vanligt vis kan du identifiera en standard instrument panel för användare om knappen **Ange som standard** inte visas i instrument panels kommando fältet.</span><span class="sxs-lookup"><span data-stu-id="57f6e-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="57f6e-106">Standard instrument panelen för användare åsidosätter alla andra standard instrument paneler, även om användarens standard instrument panel inte finns i den aktuella appen.</span><span class="sxs-lookup"><span data-stu-id="57f6e-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="57f6e-107">Använd följande lösning för att ta bort standard instrument panelen.</span><span class="sxs-lookup"><span data-stu-id="57f6e-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="57f6e-108">Skapa en ny personlig instrument panel.</span><span class="sxs-lookup"><span data-stu-id="57f6e-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="57f6e-109">Ange att den nya instrument panelen ska vara standard.</span><span class="sxs-lookup"><span data-stu-id="57f6e-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="57f6e-110">Ta bort den instrument panelen.</span><span class="sxs-lookup"><span data-stu-id="57f6e-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="57f6e-111">Instrument panelen är inställd i sitemap</span><span class="sxs-lookup"><span data-stu-id="57f6e-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="57f6e-112">Du kan ha ställt in en standard instrument panel för organisationen genom att välja en instrument panel och välja "Ange som standard" under Anpassa systemet.</span><span class="sxs-lookup"><span data-stu-id="57f6e-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="57f6e-113">Men instrument panelen som definierats i sitemap-fönstret har högre prioritet än den här instrument panelen, om användaren har åtkomst till den.</span><span class="sxs-lookup"><span data-stu-id="57f6e-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="57f6e-114">Om du vill att användarna ska kunna se den instrument panel du angett som standard organisation kan du antingen:</span><span class="sxs-lookup"><span data-stu-id="57f6e-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="57f6e-115">Ange instrument panelen i sitemap</span><span class="sxs-lookup"><span data-stu-id="57f6e-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="57f6e-116">Ta bort åtkomst till webbplats översikts instrument panelen för dessa användare</span><span class="sxs-lookup"><span data-stu-id="57f6e-116">Remove access to the sitemap defined dashboard for those users</span></span>
