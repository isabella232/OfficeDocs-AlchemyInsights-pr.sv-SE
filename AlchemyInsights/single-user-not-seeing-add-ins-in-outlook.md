---
title: En användare ser inte tillägg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198221"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>En användare ser inte tillägg i Outlook

Användaren kan vara en del av en roll som inte har rätt AppsForOfficeEnabled-parameter. Kör den här cmdleten för att ta reda på om rätt roll är associerad med användaren:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegera $false | Format-tabell -Auto roll,RollAssigneeName,RoleAssigneeType

Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
