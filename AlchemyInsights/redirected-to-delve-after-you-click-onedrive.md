---
title: OneDrive för Business Web OneDrive omdirigerar till Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571251"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="30f6d-102">Omdirigerad till Delve när du har klickat på OneDrive</span><span class="sxs-lookup"><span data-stu-id="30f6d-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="30f6d-103">Se vår detaljerade [felsökningsguide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="30f6d-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="30f6d-104">LÃ¶s problemet genom att Office 365-administratÃ¶ren ge anvÃ¤ndare rätt att skapa webbplatsen Mina webbplatser.</span><span class="sxs-lookup"><span data-stu-id="30f6d-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="30f6d-105">Detta beror på att OneDrive för företag-sidan skapas på Mina webbplatser.</span><span class="sxs-lookup"><span data-stu-id="30f6d-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="30f6d-106">Så här beviljar du denna rättighet:</span><span class="sxs-lookup"><span data-stu-id="30f6d-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="30f6d-107">Klicka på **användarprofiler**i Administrationscenter för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="30f6d-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="30f6d-108">Klicka på Hantera **användarbehörigheter**i avsnittet **Personer.**</span><span class="sxs-lookup"><span data-stu-id="30f6d-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="30f6d-109">Lägg till användare som behöver behörighet för att skapa sin webbplats för Mina webbplatser.</span><span class="sxs-lookup"><span data-stu-id="30f6d-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="30f6d-110">Som standard är den här inställningen inställd på **Alla utom externa användare**.</span><span class="sxs-lookup"><span data-stu-id="30f6d-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="30f6d-111">När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda användaren, användarna eller gruppen är markerad, bläddrar till **behörighetsavsnittet** och markerar sedan kryssrutan **bredvid Skapa personlig webbplats (krävs för personligt lagringsutrymme, nyhetsfeed och följt innehåll).**</span><span class="sxs-lookup"><span data-stu-id="30f6d-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="30f6d-112">Klicka på **OK**och sedan låta användaren bläddra till OneDrive-sidan för att skapa webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="30f6d-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
