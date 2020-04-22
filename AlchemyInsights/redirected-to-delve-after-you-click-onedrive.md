---
title: OneDrive för företag Web OneDrive omdirigerar till Delve
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
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722828"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigerad till Delve när du har klickat på OneDrive

Se vår detaljerade [felsökningsguide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

För att lösa problemet måste administratören ge användarna rätt att skapa sin webbplats Mina webbplatser. Detta beror på att sidan OneDrive för företag skapas på Mina webbplatser.

Så här beviljar du den här rättigheten:

1. Klicka på **användarprofiler**i Administrationscentret för SharePoint.

2. Klicka på Hantera **användarbehörigheter**i avsnittet **Kontakter.**

3. Lägg till användare som behöver behörighet för att skapa sin webbplats Mina webbplatser. Som standard är den här inställningen inställd **på Alla utom externa användare**.

4. När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda användaren, användarna eller gruppen är markerad, bläddrar till **behörighetsavsnittet** och markerar sedan kryssrutan **bredvid Skapa personlig webbplats (krävs för personligt lagringsutrymme, nyhetsfeed och följt innehåll)**.

5. Klicka på **OK**och låt sedan användaren bläddra till OneDrive-sidan för att skapa webbplatsen.
