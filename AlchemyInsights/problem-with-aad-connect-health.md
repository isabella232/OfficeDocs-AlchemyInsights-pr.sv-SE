---
title: Problem med AAD Connect-hälsa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483121"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Connect-hälsa

- Kontrollera att du har behörighet att utföra åtgärden. Globala administratörer har åtkomst som standard. Du kan dessutom använda rollbaserad åtkomstkontroll [för att delegera](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registreringsbehörighet för deltagare.
- Se till att de slutpunkter som krävs är aktiverade och inte blockerade på grund av brandväggen. Mer information finns i [kraven.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registreringen kan misslyckas på grund av att den utgående kommunikationen infaller på SSL-kontrollen av nätverkslagret.
- Kontrollera att du har verifierat meddelandeinställningarna för Azure AD Connect Health. Granska inställningen. Den [här](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) guiden hjälper dig att förstå hur du konfigurerar meddelandeinställningarna för hälsomeddelanden i Azure AD Connect.
- Mer information om AAD Connect Health-synkroniseringsrapporten och hur du laddar ned den finns i [synkroniseringsrapporten för objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Om du vill felsöka AAD Connect Health-varningar följer du felsökningsguiden för [AAD Connect Health-varningar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) om data freshness och för vanliga frågor, se Vanliga frågor om [AAD Connect Health-installationen.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
