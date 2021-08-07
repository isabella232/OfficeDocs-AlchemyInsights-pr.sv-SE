---
title: OneDrive för företag Webb OneDrive omdirigerar till Delve
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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923005"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeras till Delve när du klickar på OneDrive

Se vår detaljerade [felsökningsguide.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Administratören måste ge användarna rätt att skapa sina webbplatser under Mina webbplatser för att lösa problemet. Det beror på att OneDrive för företag skapas på Mina webbplatser.

Följ de här stegen för att ge den här rättigheten:

1. Klicka SharePoint användarprofiler i **administrationscentret.**

2. Klicka på **Hantera** användarbehörigheter **i avsnittet Personer.**

3. Lägg till användare som behöver behörighet för att skapa webbplatsen Mina webbplatser. Som standard är den här inställningen inställd **på Alla utom externa användare.**

4. När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda  användaren, användarna eller gruppen är markerad, bläddrar till avsnittet med behörigheter och markerar kryssrutan bredvid Skapa personlig webbplats (krävs för **personlig lagring, nyhetsfeed** och följd innehåll).

5. Klicka **på OK** och låt sedan användaren bläddra till sidan OneDrive för att skapa webbplatsen.
