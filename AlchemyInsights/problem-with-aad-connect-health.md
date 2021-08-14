---
title: Problem med AAD Anslut hälsa
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923770"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Anslut hälsa

- Se till att du har behörighet att utföra åtgärden. Globala administratörer har åtkomst som standard. Du kan dessutom använda rollbaserad [åtkomstkontroll för att delegera](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registreringsbehörighet till deltagare.
- Se till att de obligatoriska slutpunkterna är aktiverade och inte blockerade på grund av brandväggen. Mer information finns i [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreringen kan misslyckas på grund av att den utgående kommunikationen görs i SSL-kontrollen av nätverkslagret.
- Kontrollera att du har verifierat meddelandeinställningarna för Azure AD Anslut Health. Granska inställningen. Den [här](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) guiden hjälper dig att förstå hur du konfigurerar meddelandeinställningarna för Azure AD Anslut hälsomeddelanden.
- Mer information om AAD-synkroniseringsrapporten Anslut hälsosynkroniseringsrapport och hur du laddar ned den finns i [Synkroniseringsrapport för objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Om du vill felsöka AAD Anslut Health-aviseringar följer du felsökningsguiden för [AAD Anslut](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Avisering om hälsa-data och för vanliga frågor och svar finns i [Vanliga frågor om AAD Anslut Health-installation.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
