---
title: Ge användare åtkomst till SharePoint och OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736665"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Ge användare åtkomst till SharePoint och OneDrive

Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarhuvudnamn (UPN). Det nya kontot har skapats med ett annat värde PUID (Passport unika ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Andra scenariot innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare har redan inloggad i SharePoint, och har flyttats till en annan Organisationsenhet och resynced med SharePoint, kan problemet uppstå.

Lös det här problemet bör du återställa den ursprungliga UPN med åtgärderna i artikeln[återställa en användare i Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

När detta är gjort kan verifiera du användaren har admin rättigheter till OneDrive-webbplatsen genom att följa instruktionerna för att [lägga till admin tillhör en användare OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
