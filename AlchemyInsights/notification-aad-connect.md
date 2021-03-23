---
title: Meddelande om AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037235"
---
# <a name="notification-aad-connect"></a>Meddelande om AAD Connect

- Se till att du har behörighet att utföra åtgärden. Globala administratörer har åtkomst som standard. Du kan dessutom använda rollbaserad [åtkomstkontroll för att delegera](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registreringsbehörighet till deltagare.
- Se till att de obligatoriska slutpunkterna är aktiverade och inte blockerade på grund av brandväggen. Mer information finns i [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreringen kan misslyckas på grund av att den utgående kommunikationen görs i SSL-kontrollen av nätverkslagret.
- Kontrollera att du har verifierat meddelandeinställningarna för Azure AD Connect Health och granska din inställning. Information om hur du konfigurerar meddelandeinställningarna för Azure AD Connect Health-meddelanden finns i den här [guiden.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Mer information om AAD Connect Health-synkroniseringsrapporten och hur du laddar ned den finns i [Synkroniseringsrapport för objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Om du vill felsöka hälsoaviseringar för AAD Connect följer du felsökningsguiden för varningar om data i [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) och för vanliga frågor och svar finns i Vanliga frågor om installation av [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
