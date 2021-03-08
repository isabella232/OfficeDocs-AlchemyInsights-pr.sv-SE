---
title: Lösenordsloggar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527183"
---
# <a name="password-logs"></a>Lösenordsloggar

**Jag har problem med att komma åt granskningsloggar för återställning av lösenord**

Så här felsöker du problem med åtkomst till granskningsloggar för återställning av lösenord:

Se till att du har behörighet att visa granskningsloggar. 

Endast följande roller är behöriga:
 - Global administratör
 - Säkerhetsadministratör
 - Säkerhetsläsare

**Jag vill se alla granskningshändelser för återställning av lösenord från den tidpunkt jag först distribuerade**

Upp till 120 000 händelser för återställning av lösenord och registrering lagras i rapporter för de senaste 30 dagarna. Den här maxgränsen gäller för användargränssnittet när CSV-filen laddas ned. 1 miljon händelser är tillgängliga via PowerShell.
Mer information finns i länkarna nedan:

- [Självbetjäning för återställning av lösenord från API:t för Azure AD-rapporter och -händelser](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Så här laddar du ned registreringshändelser för återställning av lösenord snabbt med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Jag vill veta mer om rapporteringsfunktioner för återställning av lösenord**

Kontrollera vem som registrerar eller återställer lösenord med granskningsloggar för återställning av lösenord i Azure-portalen under **Användare och grupper.**
Mer information finns i följande länkar:

- [Översikt över rapporter för återställning av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Så här visar du rapporter om återställning av lösenord i Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Självbetjäning för återställning av lösenord från API:t för Azure AD-rapporter och -händelser](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Så här laddar du ned registreringshändelser för återställning av lösenord snabbt med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


