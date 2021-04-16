---
title: OneDrive för företag – Web OneDrive omdirigerar till Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800007"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="db25d-102">Omdirigeras till Delve när du klickar på OneDrive</span><span class="sxs-lookup"><span data-stu-id="db25d-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="db25d-103">Se vår detaljerade [felsökningsguide.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="db25d-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="db25d-104">Administratören måste ge användarna rätt att skapa sina webbplatser under Mina webbplatser för att lösa problemet.</span><span class="sxs-lookup"><span data-stu-id="db25d-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="db25d-105">Det beror på att sidan OneDrive för företag skapas på Mina webbplatser.</span><span class="sxs-lookup"><span data-stu-id="db25d-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="db25d-106">Följ de här stegen för att ge den här rättigheten:</span><span class="sxs-lookup"><span data-stu-id="db25d-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="db25d-107">Klicka på användarprofiler i administrationscentret **för** SharePoint.</span><span class="sxs-lookup"><span data-stu-id="db25d-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="db25d-108">Klicka på **Hantera** användarbehörigheter **i avsnittet Personer.**</span><span class="sxs-lookup"><span data-stu-id="db25d-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="db25d-109">Lägg till användare som behöver behörighet för att skapa webbplatsen Mina webbplatser.</span><span class="sxs-lookup"><span data-stu-id="db25d-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="db25d-110">Som standard är den här inställningen inställd **på Alla utom externa användare.**</span><span class="sxs-lookup"><span data-stu-id="db25d-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="db25d-111">När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda  användaren, användarna eller gruppen är markerad, bläddrar till avsnittet med behörigheter och markerar kryssrutan bredvid Skapa personlig webbplats (krävs för **personlig lagring, nyhetsfeed** och följd innehåll).</span><span class="sxs-lookup"><span data-stu-id="db25d-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="db25d-112">Klicka **på OK** och låt sedan användaren bläddra till OneDrive-sidan för att skapa webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="db25d-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
