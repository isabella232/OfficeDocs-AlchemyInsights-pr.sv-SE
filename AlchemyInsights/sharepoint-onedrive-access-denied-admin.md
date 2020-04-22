---
title: Felsöka nekade meddelanden om åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758537"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Felsöka nekade meddelanden i Administrationscenter för Sharepoint/OneDrive

Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett Administrationscenter för Sharepoint/OneDrive kontrollerar du att du [tilldelar användaren en licens](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Om användaren har en licens bör du också se till att de [tilldelas en administratörsroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan komma åt administratörscentren.

Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarnamn (UPN). Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller sin OneDrive har användaren ett felaktigt PUID. Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användare redan har loggat in på SharePoint och sedan flyttas till en annan organisationsenhet och synkroniseras med SharePoint, kan det här problemet uppstå.

LÃ¶s problemet genom att återställa det ursprungliga UPN med stegen i artikeln, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Om ett OneDrive- eller SharePoint-administrationscenter inte är tillgängligt för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem.  [Kontrollera instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).


