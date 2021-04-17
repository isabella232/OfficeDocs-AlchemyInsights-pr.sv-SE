---
title: Åtgärdat Microsoft 365-appar Tyvärr har vi ett meddelande om tillfälliga serverproblem
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835289"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Åtgärda meddelandet "Tyvärr har vi har tillfälliga serverproblem" i Microsoft 365-programmen

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365-appar. Se [URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå till **Starta**  >  **kör** och skriv sedan **services.msc.** Kontrollera att följande tjänster körs:
    - Nätverk anslutna enheter – automatisk konfiguration
    - Nätverkslistetjänst
    - Information om nätverksplats
    - Händelselogg i Windows

Om någon av de här tjänsterna inte körs kan du prova att starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna kommandotolken med förhöjda behörigheter:

**sfc /scannow**

Starta om datorn när det här kommandot har avslutats.

Detaljerad information finns i ["Det går tyvärr inte att ansluta till ditt konto. Försök igen senare" när du aktiverar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).