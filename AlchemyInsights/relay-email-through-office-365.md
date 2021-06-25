---
title: Vidarebefordra e-post via Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118001"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post

Mer information om alternativ och anvisningar finns i [Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post med hjälp av Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Om du har en enhet eller ett program som nyligen slutat fungera är de vanligaste problemen:

- **Autentiseringsrelaterade fel när du använder sändning via SMTP-autentiseringsklient** Vi har nyligen gjort några ändringar som rör hur SMTP-autentisering fungerar. Mer information om hur du löser problem finns i avsnittet om autentisering som inte lyckades i Åtgärda problem med [skrivare, skannrar](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)och LOB-program som skickar e-post med hjälp av Microsoft 365 eller Office 365.
- **Vi accepterar endast TLS 1.2-versionen när en säker anslutning upprättas till Office 365** Om du använder Säker anslutning (TLS) kontrollerar du att programenheten har stöd för TLS 1.2. Mer information finns i Förbereda [för TLS 1.2 i Office 365 och Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Andra problem och lösningar finns i Åtgärda problem med [skrivare, skannrar](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)och LOB-program som skickar e-post med hjälp av Microsoft 365 eller Office 365.

Om du vill se påverkade enheter går du till rapporten [SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).

**Obs!** Exchange Online kan inte hantera scenarier för massutskick. Om du vill skicka massutskick av kommersiell e-post (till exempel nyhetsbrev från kunder) bör du använda tredjepartsleverantörer som tar del av dessa tjänster.
