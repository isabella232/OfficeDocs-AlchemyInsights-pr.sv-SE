---
title: Använda DLP i transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915296"
---
# <a name="using-dlp-in-transport-rules"></a>Använda DLP i transportregler

Om du vill integrera skydd mot dataförlust (DLP) i en befintlig transport använder du villkoret "**om meddelandet innehåller...Känslig information**" i inställningarna för transportregel.

**Mer information finns i:**

- Integrerade DLP känsliga informationstyper i transportregler: [Integrera känslig information-regler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan även testa regeln med eller utan policytest med hjälp av testläget för regeln.  Du bör vänta 30 minuter efter att ha skapat regeln innan du testar den.

- Mer hittar du i [ Testa e-postflödes-/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Obs**: om du försöker implementera en ny DLP-princip med transportregler i EAC ska du använda [DLP-principer i säkerhets- och efterlevnadscenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stället.
