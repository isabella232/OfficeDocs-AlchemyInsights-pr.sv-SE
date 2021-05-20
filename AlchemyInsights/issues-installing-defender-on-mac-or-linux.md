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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539698"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problem med att installera Microsoft Defender på Mac eller Linux

**Mac**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Mac. Mer information finns i Så [här installerar du Microsoft Defender ATP för Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Granska informationen i filen: "/Bibliotek/Loggar/Microsoft/mdatp/install.log".

**Linux**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Linux. Mer information finns i [Så här installerar du MDATP för Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Kontrollera att MDATP körs i Installationen [misslyckades.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Information om hur du felsöker och löser problem om tjänsten inte körs finns i Anvisningar för att felsöka [om mdatp-tjänsten inte körs.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Information om hur du kontrollerar klientkonfigurationen, som verifierar hälsotillståndet för produkten och kör ett identifieringstest på textfilen EICAR finns i [Klientkonfiguration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Obs!** En lista över filsystem som stöds för aktivitet vid åtkomst finns i [Microsoft Defender ATP för Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)