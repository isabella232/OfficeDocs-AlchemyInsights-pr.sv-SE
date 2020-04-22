---
title: Felsöka åtkomst nekade meddelanden till OneDrive för företag-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692819"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsöka åtkomst nekade meddelanden till OneDrive för företag-webbplatser

Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarnamn (UPN). Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller sin OneDrive har användaren ett felaktigt PUID. Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare redan har loggat in på SharePoint och sedan flyttas till en annan organisationsenhet och synkroniseras med SharePoint, kan det här problemet uppstå.

1. LÃ¶s problemet genom att återställa det ursprungliga UPN med stegen i artikeln, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av dessa [steg, Ta bort en användare från listan användarinformation](). 
3. När detta är gjort kan du kontrollera att användaren har administratörsrättigheter till OneDrive-webbplatsen genom att följa stegen [i Lägg till administratör för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
