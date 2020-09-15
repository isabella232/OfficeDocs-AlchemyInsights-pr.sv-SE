---
title: Instruktioner för att dölja/ta fram grupp från adress lista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663027"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Dölj Microsoft 365 Group från Address List (GAL)

Om du vill dölja en Microsoft 365-grupp från en adress lista (GAL) i Exchange-klienter (till exempel Outlook eller OWA) använder du följande kommando i EXO skal:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Om du vill dölja Microsoft 365-gruppen som visas för Exchange-klienter använder du följande kommando i EXO skal:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

