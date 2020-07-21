---
title: Flera användare ser inte tillägg i Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198243"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Flera användare ser inte tillägg i Outlook

Om du testar Outlook-tillägg och ingen visas, som ett första felsökningssteg, använder du **Get-OrganizationConfig** PowerShell-cmdlet för att fråga parametern _AppsForOfficeEnabled._ Om frågan returnerar ett värde i **False**anger du den här parametern till **True** med hjälp av **cmdlet Set-OrganizationConfig,** så att tillägg visas som förväntat.

Vi rekommenderar inte att parametern _AppsForOfficeEnabled_ är inställd på **False**. Värdet **False** åsidosätter alla ovanstående inställningar för administratörs- och användarroll och förhindrar att nya appar aktiveras av alla användare i organisationen.

Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).