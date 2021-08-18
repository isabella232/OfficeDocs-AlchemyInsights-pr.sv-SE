---
title: Problem med att installera Microsoft Defender på Mac eller Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898626"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problem med att installera Microsoft Defender på Mac eller Linux

**Mac**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Mac. Mer information finns i Installera [Microsoft Defender ATP för Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Granska informationen i filen: "/Bibliotek/Loggar/Microsoft/mdatp/install.log".

**Linux**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Linux. Mer information finns i Installera [MDATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Du kan kontrollera att MDATP-tjänsten är igång genom att gå till [Installationen misslyckades.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Information om hur du felsöker och löser problem om tjänsten inte körs finns i Anvisningar för att felsöka [om mdatp-tjänsten inte körs.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Information om hur du kontrollerar klientkonfigurationen, som verifierar produktens hälsa och kör ett identifieringstest på textfilen EICAR finns i [Klientkonfiguration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Obs!** En lista över filsystem som stöds för aktivitet vid åtkomst finns i [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)