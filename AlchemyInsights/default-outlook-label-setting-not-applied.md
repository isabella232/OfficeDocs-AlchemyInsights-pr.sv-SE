---
title: Standardinställningen Outlook etikett används inte
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
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455085"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standardinställningen Outlook etikett används inte

Om standardinställningarna för Outlook-etiketter inte tillämpas på rätt sätt och en annan etikett eller ingen etikett används, kan ett känt problem (MC277818) uppstå och du bör göra något av följande två alternativ för att lösa problemet:

**Alternativ 1:**

1. Gå till Microsoft 365 Kompatibilitetscenter > **Solutions**  >  **Information Protection**.
1. Välj **Etikettprinciper** och välj den etikettprincip du behöver redigera (**OutlookDefaultlabel-inställningen** är inte korrekt inställd för den etikettprincip som gäller. Kör **Get-labelpolicy för** att visa den här inställningen) och välj **sedan Redigera princip**.
1. Välj **Nästa** tills du ser inställningen Använd den här standardetiketten för e-postmeddelanden **,** som är tillgänglig om du väljer Kräv att användare använder en etikett för arv av e-postmeddelanden och dokument i dialogrutan **Principinställningar.** 
1. I dialogrutan **Använd en standardetikett för** dokument väljer du **Ingen** i listrutan.
1. Välj **Nästa** och **Skicka för** att spara etikettinställningarna.

**Alternativ 2:**

I Säkerhets- och efterlevnadscenter [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)använder du Set-LabelPolicy-kommandoleten för att ändra **OutlookDefaultlabel** till **Ingen** på {OutlookDefaultLabel="None"}.

Kör: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Mer information om standardetiketter för Outlook finns [i Ange en annan standardetikett för Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).