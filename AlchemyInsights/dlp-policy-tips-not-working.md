---
title: DLP-principtips fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932604"
---
# <a name="dlp-policy-tip-issues"></a>Problem med DLP-principtips

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**Tips för DLP-policy**

När du använder **DLP-principer**kan användare meddelas om en policyöverträdelse med **principtips**. Administratörer kan konfigurera principtips som ska visas när de testar sin DLP-princip eller när principen är i fullständigt tvingande läge.
  
Så här konfigurerar du principtips för DLP-principen i säkerhets- och efterlevnadscentret i fullständigt tvingande läge:
  
- Kontrollera att principtips har **aktiverats** på DLP-regeln med hjälp av stegen [här](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Se till att **ditt innehåll matchar** vad som **krävs** för att utlösa regeln som beskrivs i den här artikeln [här](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Principtips visas i både OWA och Outlook. När du använder **Outlook 2013 eller senare**visas dock principtips endast under vissa förhållanden. Dessa villkor visas här: [Villkor som stöds för Outlook 2013 eller senare för att visa principtips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Mer information om DLP-principtips finns i: [Visa principtips för DLP-principer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  