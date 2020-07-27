---
title: Flera användare får åtkomst nekad fel när du lägger till tillägg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424176"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Flera användare får åtkomst nekad fel när du lägger till tillägg i Outlook

Du kan ange vilka administratörer i organisationen som har behörighet att installera och hantera tillägg för Outlook. Du kan också ange vilka användare i organisationen som har behörighet att installera och hantera tillägg för eget bruk.

Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Om du vill kontrollera att du har tilldelat behörigheter för en användare ersätter du <Role Name> med namnet på rollen som ska verifieras och kör följande kommando i Exchange Online PowerShell:

Get-ManagementRoleAssignment -Roll " <Role Name> " -GetEffectiveUsers

I det här exemplet visas hur du verifierar vem du har tilldelat behörigheter för att installera tillägg från Office Store för organisationen.

Powershell

-Roll "Org Marketplace Apps" -GetEffectiveUsers

I resultatet, Get-ManagementRoleAssignment, granska posterna i kolumnen Effektiva användare.

Detaljerad syntax- och parameterinformation finns i [Hämta-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 