---
title: Klassiska SharePoint-granskningsloggrapporter
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509618"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Granskningsloggar för SharePoint och OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassiska granskningsloggar i SharePoint

SPO:s äldre granskning migrerades till Unified Audit Log (UAL). Alla SPO-äldre granskningsrapporter kommer nu att drivas via UAL och de äldre granskningssignalerna har migrerats till UAL.

Viktiga ändringar:

* Trimning är INTE tillgänglig som en funktion.
* Att välja specifika händelser att granska är INTE tillgängligt. Se [det här dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.
* Alternativet **Plats** under **Anpassade rapporter** är INTE tillgängligt.
* Alternativet **Öppna eller hämta dokumenthändelser** är INTE tillgängligt.

[Konfigurera granskningsinställningar för en webbplatssamling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- och OneDrive-moderna enhetliga granskningsloggar från efterlevnad

* [Aktivera/inaktivera enhetlig granskningsloggning](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.

Använd granskningsloggning för att kontrollera aktiviteten för filen eller mapparna, mapparna, användaren/kanna, behörigheterna:

* [Fil- och sidaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter för att dela och få åtkomst till begäran](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter för webbplatsadministration](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Mer information om hur du hämtar dessa händelser finns i [Sök i granskningsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
