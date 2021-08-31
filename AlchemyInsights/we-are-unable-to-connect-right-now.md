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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744613"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Åtgärda meddelandet Microsoft 365 om att det inte går att ansluta just nu

Obs! Om du använder en äldre version av Windows (t.ex. Windows 7 SP1, Windows Server 2008 R2) använder du den enkla [korrigeringen](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) för att aktivera TLS 1.2 som standard. Mer information finns i Uppdatering för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365 program. Se [Microsofts URL:er och IP-adressintervall.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Gå till **Starta**  >  **kör** och skriv sedan **services.msc.** Kontrollera att följande tjänster körs:
    - Nätverk anslutna enheter – automatisk konfiguration
    - Nätverkslistetjänst
    - Information om nätverksplats
    - Windows Händelselogg

Om någon av de här tjänsterna inte körs kan du prova att starta den. Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:

**sfc /scannow**

Starta om datorn när det här kommandot har avslutats.

Detaljerad information finns i ["Det går tyvärr inte att ansluta till ditt konto. Försök igen senare" när du aktiverar ett Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).