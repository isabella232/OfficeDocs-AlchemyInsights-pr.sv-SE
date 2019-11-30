---
title: Åtgärda Office-appar tyvärr, vi har tillfälliga Server problem meddelande
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628008"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Fastställande av Office Apps "Tyvärr, vi har tillfälliga Server problem" meddelande

Om det här meddelandet visas provar du följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internet-åtkomst till Office-appar. Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå till **Start** > **Run**och skriv **Services. msc**. Kontrollera att följande tjänster körs:
    - Automatisk konfigurering av nätverksanslutna enheter
    - Network List Service
    - Nätverksplats medvetenhet
    - Händelseloggen för Windows

Om någon av dessa tjänster inte körs försöker du starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:

**sfc/scannow**

När det här kommandot har slutförts startar du om datorn.

Mer information finns i ["Tyvärr kan vi inte ansluta till ditt konto. Försök igen senare "felmeddelande när du aktiverar Office från Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).