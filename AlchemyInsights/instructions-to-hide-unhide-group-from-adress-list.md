---
title: Instruktioner för att dölja/Visa grupp från adresslista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768956"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Dölj Office 365 grupp från adresslista (GAL)

Om du vill dölja en Office 365-grupp från adresslistor (GAL) för Exchange-klienter (till exempel Outlook eller OWA) använder du följande kommando i EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Om du vill dölja Office 365-gruppen från att vara synlig för Exchange-klienter använder du följande kommando i EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

