---
title: Felsöka åtkomst nekade meddelanden
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767681"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Felsöka åtkomst nekade meddelanden i administrations centret för SharePoint/OneDrive

Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett administrations Center för SharePoint/OneDrive måste du [tilldela en licens till användaren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Om användaren har en licens bör du också kontrol lera att de [tilldelats en administratörs roll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har åtkomst till administrations centret.

Det här problemet kan även uppstå när en användare tas bort och återskapas med samma huvud namn (UPN). Det nya kontot skapas med ett annat PUID-värde (unikt ID). När användaren försöker komma åt en webbplats samling eller deras OneDrive har användaren felaktigt PUID. Ett andra scenario inkluderar profilsynkronisering med en Active Directory-organisationsenhet (OU). Om användare redan har loggat in i SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan de uppleva det här problemet.

Lös problemet genom att återställa den ursprungliga UPN-informationen enligt anvisningarna i artikeln [återställa en användare i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

OBS! om ett OneDrive-eller SharePoint-administrationsobjekt inte är tillgängligt för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänst problem.  [Kontrol lera instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).


