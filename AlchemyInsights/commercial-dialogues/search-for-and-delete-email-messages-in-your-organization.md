---
title: Söka efter och ta bort e-postmeddelanden i din organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948901"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Söka efter och ta bort e-postmeddelanden i din organisation

Gör så här:

1. Om du inte är global administratör måste du lägga till ditt konto i rollgruppen **för eDiscovery-hanteraren** eller rollen För efterlevnadssökning för att söka efter **meddelanden.** Om du vill ta bort meddelanden måste du gå med i **rollgruppen Organisationshantering** eller rollen **För hantering av sökning och rensning.** Behörigheter till de här rollerna tilldelas [i Säkerhets- & säkerhets- och efterlevnadscenter.](https://protection.office.com)
2. [Skapa en innehållssökning för](https://docs.microsoft.com/office365/securitycompliance/content-search) att hitta det meddelande du vill ta bort.
3. [Anslut till Säkerhets- och efterlevnadscenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Om du använder MFA följer du de här anvisningarna: Anslut säkerhets- & Säkerhets- och [efterlevnadscenter med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Ta bort meddelandet: kör `New-ComplianceSearchAction` cmdleten för att ta bort meddelandet. Borttagna meddelanden flyttas till en användares återställningsbara objekt-mapp. Ett exempelkommando finns i Steg [3: Ta bort meddelandet.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
