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
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeras till Delve när du klickar på OneDrive

Se vår detaljerade [felsökningsguide.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Administratören måste ge användarna rätt att skapa sina webbplatser under Mina webbplatser för att lösa problemet. Det beror på att sidan OneDrive för företag skapas på Mina webbplatser.

Följ de här stegen för att ge den här rättigheten:

1. Klicka på användarprofiler i administrationscentret **för** SharePoint.

2. Klicka på **Hantera** användarbehörigheter **i avsnittet Personer.**

3. Lägg till användare som behöver behörighet för att skapa webbplatsen Mina webbplatser. Som standard är den här inställningen inställd **på Alla utom externa användare.**

4. När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda  användaren, användarna eller gruppen är markerad, bläddrar till avsnittet med behörigheter och markerar kryssrutan bredvid Skapa personlig webbplats (krävs för **personlig lagring, nyhetsfeed** och följd innehåll).

5. Klicka **på OK** och låt sedan användaren bläddra till OneDrive-sidan för att skapa webbplatsen.
