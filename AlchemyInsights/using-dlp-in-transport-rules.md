---
title: Använda DLP i transportregler
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827234"
---
# <a name="using-dlp-in-transport-rules"></a>Använda DLP i transportregler

Om du vill integrera skydd mot dataförlust (DLP) i en befintlig transport använder du villkoret "**om meddelandet innehåller...Känslig information**" i inställningarna för transportregel.

**Mer information finns i:**

- Integrerade DLP känsliga informationstyper i transportregler: [Integrera känslig information-regler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan även testa regeln med eller utan policytest med hjälp av testläget för regeln.  Du bör vänta 30 minuter efter att ha skapat regeln innan du testar den.

- Mer hittar du i [ Testa e-postflödes-/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Obs**: om du försöker implementera en ny DLP-princip med transportregler i EAC ska du använda [DLP-principer i säkerhets- och efterlevnadscenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stället.
