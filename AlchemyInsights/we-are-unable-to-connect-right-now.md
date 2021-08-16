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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998190"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Åtgärda meddelandet Microsoft 365 om att det inte går att ansluta just nu

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365 program. Se [Microsofts URL:er och IP-adressintervall.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Gå till **Starta**  >  **kör** och skriv sedan **services.msc.** Kontrollera att följande tjänster körs:
    - Nätverk anslutna enheter – automatisk konfiguration
    - Nätverkslistetjänst
    - Information om nätverksplats
    - Windows Händelselogg

Om någon av de här tjänsterna inte körs kan du prova att starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna kommandotolken med förhöjda behörigheter:

**sfc /scannow**

Starta om datorn när det här kommandot har avslutats.

Detaljerad information finns i ["Det går tyvärr inte att ansluta till ditt konto. Försök igen senare" när du aktiverar ett Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).