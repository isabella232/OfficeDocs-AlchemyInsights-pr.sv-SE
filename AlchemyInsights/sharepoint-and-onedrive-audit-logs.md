---
title: Klassiska redovisnings rapporter för SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662226"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Gransknings loggar för SharePoint och OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassiska SharePoint-gransknings loggar

SPO Legacy-granskning migrerades till Unified audit log (UAL). Alla SPO-gransknings rapporter kommer nu att startas med UAL och de äldre gransknings signalerna har migrerats till UAL.

Viktiga ändringar:

* Trimning är inte tillgänglig som en funktion.
* Det går inte att välja specifika händelser som ska granskas. I [det här dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) finns en fullständig lista över granskade händelser som är tillgängliga som standard.
* Alternativet **plats** under **anpassade rapporter** är inte tillgängligt.
* Alternativet för att **Öppna eller ladda ned dokument** händelser är inte tillgängligt.

[Konfigurera gransknings inställningar för en webbplats samling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint-och OneDrive-moderna enhetliga redovisnings loggar från efterlevnad

* [Aktivera/inaktivera enhetlig gransknings loggning](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Det krävs ingen ytterligare konfiguration i SharePoint eller OneDrive.

Använd gransknings loggnings sökning för att kontrol lera aktivitet för filer, mappar, användare, behörigheter:

* [Fil-och sid aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter för delning och åtkomstbegäran](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsuppgift](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter för webbplats administration](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Mer information om hur du hämtar de här händelserna finns i [söka i gransknings loggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
