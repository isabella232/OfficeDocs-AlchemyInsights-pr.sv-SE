---
title: Aktiveringsproblem - Vi kan inte ansluta just nu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716190"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Åtgärda meddelandet "Vi kan inte ansluta just nu"

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Office-appar. Se [Microsofts url:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå till > **Startkörning**och skriv sedan **services.msc**. **Start** Kontrollera att alla följande tjänster körs:
    - Automatisk installation av nätverksanslutna enheter
    - Tjänsten Nätverkslista
    - Medvetenhet om nätverksplats
    - Windows-händelselogg

Om en av dessa tjänster inte körs försöker du starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:

**sfc /scannow**

När det här kommandot är klart startar du om datorn.

Detaljerad information finns i ["Tyvärr, vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).