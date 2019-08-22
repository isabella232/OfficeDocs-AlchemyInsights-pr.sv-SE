---
title: 'Felsökning: åtkomst nekad meddelanden'
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503561"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Felsökning: åtkomst nekad meddelanden i Sharepoint OneDrive/Admin Center

Om du får meddelandet åtkomst nekad när du försöker bläddra till en Sharepoint OneDrive/Admin Center, kontrollera att du [tilldela en licens till användaren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Om användaren har en licens, bör du försäkra dig om att de är [tilldelade en administratör](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan komma åt admin Center.

Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarhuvudnamn (UPN). Det nya kontot har skapats med ett annat värde PUID (Passport unika ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Andra scenariot innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare har redan inloggad i SharePoint, och har flyttats till en annan Organisationsenhet och resynced med SharePoint, kan problemet uppstå.

Lös det här problemet, bör du återställa den ursprungliga UPN med åtgärderna i artikeln [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Anmärkning: Om ett OneDrive eller SharePoint Admin center inte är tillgängligt för flera användare som tidigare hade åtkomst, kan det finnas en tillfällig service problem.  [Kontrollera att tjänsten hälsa instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).


