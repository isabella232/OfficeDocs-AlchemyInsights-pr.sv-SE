---
title: OneDrive för företag – webb OneDrive-omdirigering till Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776398"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigerad till Delve efter att du klickat på OneDrive

Se vår detaljerade [fel söknings guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

För att lösa problemet måste administratören ge användare behörighet att skapa webbplatsen mina webbplatser. Det beror på att sidan OneDrive för företag skapas på mina webbplatser.

Följ de här anvisningarna för att bevilja denna rättighet:

1. I administrations centret för SharePoint klickar du på **användar profiler**.

2. Klicka på **Manage User Permissions**i avsnittet **personer** .

3. Lägg till användare som behöver behörigheter för att skapa webbplatsen mina webbplatser. Den här inställningen är inställd på **alla utom externa användare**.

4. När du har lagt till användaren, användare eller gruppen kontrollerar du att den tillagda användaren, användaren eller gruppen är markerad, bläddrar till avsnittet **behörigheter** och markerar sedan kryss rutan bredvid **skapa personlig webbplats (obligatoriskt för personlig lagring, nyhetsfeed och följt innehåll)**.

5. Klicka på **OK**och låt sedan användaren Bläddra till OneDrive-sidan och skapa webbplatsen.
