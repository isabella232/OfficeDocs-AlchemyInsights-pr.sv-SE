---
title: Felsöka åtkomst nekad-meddelanden
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751294"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Felsöka åtkomst nekad meddelanden i SharePoint/OneDrive administratörs Center

Om du får ett meddelande om nekad åtkomst när du försöker bläddra till en SharePoint/OneDrive administratörs Center, se till att du [tilldelar en licens till användaren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Om användaren har en licens, bör du också se till att de har [tilldelats en administratörsroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan komma åt admin Centers.

Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarens huvudnamn (UPN). Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID. Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU). Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan det här problemet uppstå.

Lös det här problemet bör du återställa det ursprungliga UPN-namnet med stegen i artikeln, [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Om ett OneDrive-eller SharePoint-administratörscenter inte är tillgängligt för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänstproblem.  [Kontrollera den service Health instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).


