---
title: Aktiverings problem – vi kan inte ansluta just nu
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726001"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Åtgärdar Microsoft 365-apparna "det går inte att ansluta just nu"

Om du får det här meddelandet kan du prova följande:

1. Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Internet åtkomst till Microsoft 365-appar. Se [URL-adresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå till **Start**  >  **Kör**och skriv **Services. msc**. Kontrol lera att följande tjänster körs:
    - Automatisk konfiguration av nätverksanslutna enheter
    - Tjänsten nätverks lista
    - Nätverks plats medvetenhet
    - Windows-händelseloggen

Om någon av de här tjänsterna inte körs kan du försöka starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommando tolk med förhöjda behörigheter:

**sfc/scannow**

Starta om datorn när det här kommandot är klart.

Detaljerad information finns i ["det går inte att ansluta till ditt konto. Försök igen senare "visas när du aktiverar Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).