---
title: Klassiska SharePoint-granskningsloggrapporter
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068041"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Granskningsloggar för SharePoint och OneDrive

**SharePoint och OneDrive moderna enhetliga granskningsloggar från efterlevnad**

- [Aktivera/inaktivera enhetlig granskningsloggning](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.

- Använd granskningsloggning Sök för att kontrollera aktiviteten för filen (s), mapp (ar), användare (s), behörigheter:

    - [Fil-och sid aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Mappaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Aktiviteter för delning och åtkomstbegäran](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Aktiviteter för Webbplatsadministration](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Mer information om hur du hämtar dessa händelser finns [i söka i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Klassiska SharePoint-granskningsloggar**

Vi migrerade SPO Legacy Auditing till Unified audit log (UAL). Detta innebär i huvudsak att alla SPO äldre granskningsrapporter nu kommer att drivas via UAL och att de äldre gransknings signalerna har migrerats till UAL.

Viktiga ändringar:

- Trimning som en funktion är inte tillgänglig.
- Avsnittet där du väljer specifika händelser för granskning är inte tillgängligt. Se [detta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.
- Alternativet "plats" under **anpassade rapporter** är inte tillgängligt. 
- "Öppna eller ladda ned dokument" händelser är inte tillgängliga. 

