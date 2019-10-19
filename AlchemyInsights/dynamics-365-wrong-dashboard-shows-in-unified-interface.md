---
title: Dynamics 365-fel instrumentpanel visas i Dynamics 365 enhetligt gränssnitt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528569"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="54401-102">Fel instrumentpanel visas i Dynamics 365 enhetligt gränssnitt</span><span class="sxs-lookup"><span data-stu-id="54401-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="54401-103">Det finns flera anledningar till att du kan se en annan instrumentpanel än den du förväntar dig:</span><span class="sxs-lookup"><span data-stu-id="54401-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="54401-104">Användaren har angett en standardinstrumentpanel för användare</span><span class="sxs-lookup"><span data-stu-id="54401-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="54401-105">Vanligtvis kan du identifiera en standardinstrumentpanel för användare anges om knappen **Ange som standard** inte visas i instrumentpanelens kommandofält.</span><span class="sxs-lookup"><span data-stu-id="54401-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="54401-106">Standardinstrumentpanelen för användare åsidosätter alla andra standardinstrumentpaneler, även om användarens standardinstrumentpanel inte finns i den aktuella appen.</span><span class="sxs-lookup"><span data-stu-id="54401-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="54401-107">Använd följande lösning för att ta bort deras standardinstrumentpanel.</span><span class="sxs-lookup"><span data-stu-id="54401-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="54401-108">Skapa en ny personlig instrumentpanel.</span><span class="sxs-lookup"><span data-stu-id="54401-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="54401-109">Ange den nya instrumentpanelen som Användarstandard.</span><span class="sxs-lookup"><span data-stu-id="54401-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="54401-110">Ta bort den instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="54401-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="54401-111">Instrumentpanelen anges i webbplatsöversikten</span><span class="sxs-lookup"><span data-stu-id="54401-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="54401-112">Du kan ha ställt in en standardinstrumentpanel för organisationen genom att välja en instrumentpanel och välja "Ange som standard" under "anpassa systemet".</span><span class="sxs-lookup"><span data-stu-id="54401-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="54401-113">Men instrumentpanelen som definierats i sitemap-designern kommer att ha företräde framför den här instrumentpanelen, om användaren har åtkomst till den.</span><span class="sxs-lookup"><span data-stu-id="54401-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="54401-114">Om du vill att användarna ska se den instrumentpanel som du har angett som standard för organisationen kan du antingen:</span><span class="sxs-lookup"><span data-stu-id="54401-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="54401-115">Ange den instrumentpanelen i webbplatsöversikten</span><span class="sxs-lookup"><span data-stu-id="54401-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="54401-116">Ta bort åtkomsten till webbplatsöversikten definierad instrumentpanel för dessa användare</span><span class="sxs-lookup"><span data-stu-id="54401-116">Remove access to the sitemap defined dashboard for those users</span></span>
