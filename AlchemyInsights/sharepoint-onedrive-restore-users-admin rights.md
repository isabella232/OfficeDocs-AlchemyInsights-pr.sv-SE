---
title: Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507829"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser

Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarhuvudnamn (UPN). Det nya kontot har skapats med ett annat värde PUID (Passport unika ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Andra scenariot innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare har redan inloggad i SharePoint, och har flyttats till en annan Organisationsenhet och resynced med SharePoint, kan problemet uppstå.

1. Lös det här problemet bör du återställa den ursprungliga UPN med åtgärderna i artikeln[återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av dessa steg [tar bort en användare från användarinformationslistan](). 
3. När detta är gjort kan verifiera du användaren har admin rättigheter till OneDrive-webbplatsen genom att följa instruktionerna för att [lägga till admin tillhör en användare OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
