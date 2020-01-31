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
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigerad till Delve när du har klickat på OneDrive

Se vår detaljerade [felsökningsguide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

LÃ¶s problemet genom att Office 365-administratÃ¶ren ge anvÃ¤ndare rätt att skapa webbplatsen Mina webbplatser. Detta beror på att OneDrive för företag-sidan skapas på Mina webbplatser.

Så här beviljar du denna rättighet:

1. Klicka på **användarprofiler**i Administrationscenter för SharePoint.

2. Klicka på Hantera **användarbehörigheter**i avsnittet **Personer.**

3. Lägg till användare som behöver behörighet för att skapa sin webbplats för Mina webbplatser. Som standard är den här inställningen inställd på **Alla utom externa användare**.

4. När du har lagt till användaren, användarna eller gruppen kontrollerar du att den tillagda användaren, användarna eller gruppen är markerad, bläddrar till **behörighetsavsnittet** och markerar sedan kryssrutan **bredvid Skapa personlig webbplats (krävs för personligt lagringsutrymme, nyhetsfeed och följt innehåll).**

5. Klicka på **OK**och sedan låta användaren bläddra till OneDrive-sidan för att skapa webbplatsen.
