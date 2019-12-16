---
title: Felsöka åtkomst nekad meddelanden till OneDrive för Business-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051623"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsöka åtkomst nekad meddelanden till OneDrive för Business-webbplatser

Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarens huvudnamn (UPN). Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan det här problemet uppstå.

1. Lös det här problemet bör du återställa den ursprungliga UPN med stegen i artikeln, [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av dessa steg, [ta bort en användare från listan användarinformation](). 
3. När detta är gjort kan du kontrollera att användaren har administratörsrättigheter till webbplatsen för OneDrive genom att följa stegen för att [lägga till admin för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Mer information om behörighetsnivåer finns i artikeln [förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
