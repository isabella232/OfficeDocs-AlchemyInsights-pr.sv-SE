---
title: Dölja eller dölja Office 365-grupper eller -team i adresslistan
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811474"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Dölja eller dölja Office 365-grupper eller -team i adresslistan

Använd följande EXO PowerShell-kommando för att dölja eller dölja Office 365-grupper från adresslistor (GAL) för Exchange-klienter (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Använd följande EXO PowerShell-kommando för att dölja eller dölja Office365-gruppen/-teamen från Exchange-klienter (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaljerade instruktioner finns i Dölja [Office 365-grupper från GAL och Exchange-klienter.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
