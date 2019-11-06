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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992636"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Granskningsloggar för SharePoint och OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassiska SharePoint-granskningsloggar

SPO Legacy Auditing migrerades till Unified audit log (UAL). Alla SPO äldre granskningsrapporter kommer nu att drivas via UAL och de äldre gransknings signalerna har migrerats till UAL.

Viktiga ändringar:

* Trimning är inte tillgänglig som en funktion.
* Det går inte att välja specifika händelser för granskning. Se [detta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.
* Alternativet **plats** under **anpassade rapporter** är inte tillgängligt.
* Alternativet **Öppna eller hämta dokument** händelser är inte tillgängligt.

[Konfigurera granskningsinställningar för en webbplatssamling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint och OneDrive moderna enhetliga granskningsloggar från efterlevnad

* [Aktivera/inaktivera enhetlig granskningsloggning](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.

Använd granskningsloggning Sök för att kontrollera aktiviteten för filen (s), mapp (ar), användare (s), behörigheter:

* [Fil-och sid aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter för delning och åtkomstbegäran](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter för Webbplatsadministration](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Mer information om hur du hämtar dessa händelser finns [i söka i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
