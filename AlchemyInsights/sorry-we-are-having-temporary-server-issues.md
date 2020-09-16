---
title: Åtgärda Microsoft 365-appar vi har tyvärr problem med tillfällig Server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758263"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Åtgärdar ett meddelande om att Microsoft 365-apparna "Vi har tillfälliga Server problem"

Om du får det här meddelandet kan du prova följande:

1. Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Internet åtkomst till Microsoft 365-appar. Se [URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå till **Start**  >  **Kör**och skriv **Services. msc**. Kontrol lera att följande tjänster körs:
    - Automatisk konfiguration av nätverksanslutna enheter
    - Tjänsten nätverks lista
    - Nätverks plats medvetenhet
    - Windows-händelseloggen

Om någon av de här tjänsterna inte körs kan du försöka starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommando tolk med förhöjda behörigheter:

**sfc/scannow**

Starta om datorn när det här kommandot är klart.

Detaljerad information finns i ["det går inte att ansluta till ditt konto. Försök igen senare "när du aktiverar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).