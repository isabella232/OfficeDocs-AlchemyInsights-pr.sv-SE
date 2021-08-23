---
title: Aviseringar saknas på fliken Aviseringar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454965"
---
# <a name="alerts-missing-from-alerts-tab"></a>Aviseringar saknas på fliken Aviseringar

Fliken **Aviseringar** fungerar baserat på konfigurations- och aktiverade principer från appstyrningsportalen i klientorganisationen. In-to-box policies in App Governance also must beactivated to let signals flow to **the Alerts** tab. 

Bekräfta att aviseringen har skapats:

1. Gå till principer för [appstyrning](https://compliance.microsoft.com/m365appprotection?viewid=policies) och bekräfta att du har skapat minst en aktiv princip eller granskningsprincip.

1. Markera principen och se till att redigera **i** den utfällliga rutan. 

1. Kontrollera principkonfigurationen för att bekräfta att en avisering borde ha skapats baserat på en principhändelse som initierades för mer än 24 timmar sedan.

Mer information om varningar i appstyrning finns i Komma igång med identifiering och åtgärd av [apphot.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)