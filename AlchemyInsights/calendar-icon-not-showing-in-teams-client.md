---
title: Kalender-ikonen visas inte i Teams-klienten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932383"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalender-ikonen visas inte i Teams-klienten

Fliken Kalender i Teams kräver åtkomst till en Exchange-postlåda via Exchange webbtjänster. Exchange-postlådan kan vara online eller lokal. För online-användare som inte kan se fliken Kalender ser du till att de [har licens för en Exchange Online-postlåda och att postlådan är aktiverad](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Det kan vara problem med nätverket om användaren har en giltig postlåda i Exchange Online men fortfarande inte kan se fliken Kalender. Använd [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) och kör **Anslutningstest för Microsoft Exchange webbtjänster** för den påverkade användaren.

Kontrollera slutligen [Teams-appar – principer för programkonfiguration](https://admin.teams.microsoft.com/policies/app-setup) för att säkerställa att kalenderprogrammet inte har tagits bort från principen som används för användaren (troligen **globala (standard för hela organisationen)**.

Om användarna är finns lokalt måste du bekräfta att hybridkonfigurationen är felfri. Använd [Guiden för hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) för felsökning.

Observera att [Teams kräver Exchange 2016 CU3 eller senare](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
