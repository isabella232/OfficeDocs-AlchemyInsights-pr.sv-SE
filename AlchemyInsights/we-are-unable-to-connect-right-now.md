---
title: Aktiveringsproblem – det går inte att ansluta just nu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806460"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Åtgärda meddelandet "Det går inte att ansluta just nu" i Microsoft 365-programmen

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365-appar. Se [Microsofts URL:er och IP-adressintervall.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Gå till **Starta**  >  **kör** och skriv sedan **services.msc.** Kontrollera att följande tjänster körs:
    - Nätverk anslutna enheter – automatisk konfiguration
    - Nätverkslistetjänst
    - Information om nätverksplats
    - Händelselogg i Windows

Om någon av de här tjänsterna inte körs kan du prova att starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna kommandotolken med förhöjda behörigheter:

**sfc /scannow**

Starta om datorn när det här kommandot har avslutats.

Detaljerad information finns i ["Det går tyvärr inte att ansluta till ditt konto. Försök igen senare" när du aktiverar Office från Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)