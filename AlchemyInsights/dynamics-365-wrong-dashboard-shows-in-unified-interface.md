---
title: Dynamics 365 - fel instrumentpanelen visas i Dynamics 365 enhetligt gränssnitt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748899"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="1457c-102">Fel instrumentpanelen visas i Dynamics 365 enhetligt gränssnitt</span><span class="sxs-lookup"><span data-stu-id="1457c-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="1457c-103">Det finns flera orsaker till varför du kan se en annan instrumentpanel än förväntat:</span><span class="sxs-lookup"><span data-stu-id="1457c-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="1457c-104">Användaren har angett en standard</span><span class="sxs-lookup"><span data-stu-id="1457c-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="1457c-105">Vanligtvis kan du identifiera en användare standardinstrumentpanel anges om knappen **Ange som standard** inte visas i kommandofältet instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="1457c-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="1457c-106">Användaren standardinstrumentpanel åsidosätts alla standard-instrumentpaneler även om användarinstrumentpanel standard inte är den aktuella appen.</span><span class="sxs-lookup"><span data-stu-id="1457c-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="1457c-107">Använd följande lösning ta bort deras standardinstrumentpanel.</span><span class="sxs-lookup"><span data-stu-id="1457c-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="1457c-108">Skapa en ny personlig instrumentpanel.</span><span class="sxs-lookup"><span data-stu-id="1457c-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="1457c-109">Ange den nya instrumentpanelen som standard.</span><span class="sxs-lookup"><span data-stu-id="1457c-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="1457c-110">Ta bort den här instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="1457c-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="1457c-111">Instrumentpanelen är inställd i Webbplatsöversikt</span><span class="sxs-lookup"><span data-stu-id="1457c-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="1457c-112">Du kan ha angett en standardinstrumentpanel för organisationen genom att välja en instrumentpanel och välja 'Ange som standard ”under” Anpassa systemet ”.</span><span class="sxs-lookup"><span data-stu-id="1457c-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="1457c-113">Men instrumentpanelen som definierats i sitemap designer har högre prioritet än den här instrumentpanelen om användaren har åtkomst till den.</span><span class="sxs-lookup"><span data-stu-id="1457c-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="1457c-114">Om du vill att användare kan visa på instrumentpanelen som du angett som Organisationsstandard, kan du antingen:</span><span class="sxs-lookup"><span data-stu-id="1457c-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="1457c-115">Ange att instrumentpanelen i Webbplatsöversikt</span><span class="sxs-lookup"><span data-stu-id="1457c-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="1457c-116">Ta bort åtkomst till instrumentpanelen sitemap definieras för dessa användare</span><span class="sxs-lookup"><span data-stu-id="1457c-116">Remove access to the sitemap defined dashboard for those users</span></span>
