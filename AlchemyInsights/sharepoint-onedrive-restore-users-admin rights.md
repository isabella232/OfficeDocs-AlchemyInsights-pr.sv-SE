---
title: Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354815"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser

Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarhuvudnamn (UPN). Det nya kontot har skapats med ett annat värde PUID (Passport unika ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Andra scenariot innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare har redan inloggad i SharePoint, och har flyttats till en annan Organisationsenhet och resynced med SharePoint, kan problemet uppstå.

Lös det här problemet bör du återställa den ursprungliga UPN med åtgärderna i artikeln[återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

När detta är gjort kan verifiera du användaren har admin rättigheter till OneDrive-webbplatsen genom att följa instruktionerna för att [lägga till admin tillhör en användare OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
