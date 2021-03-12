---
title: Problem med installationen av Microsoft Defender på Mac eller Linux
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714317"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problem med installationen av Microsoft Defender på Mac eller Linux

**Mac**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Mac. Mer information finns i Installera [Microsoft Defender ATP för Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Granska informationen i filen: "/Bibliotek/Loggar/Microsoft/mdatp/install.log".

**Linux**

- Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Linux. Mer information finns i Installera [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Kontrollera att MDATP-tjänsten körs genom att gå till [Installationen misslyckades.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Information om hur du felsöker och löser problem om tjänsten inte körs finns i Anvisningar för att felsöka [om mdatp-tjänsten inte körs.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Instruktioner för hur du kontrollerar klientkonfigurationen, som verifierar hälsotillståndet för produkten och kör ett identifieringstest på TEXTfilen EICAR, finns i [Klientkonfiguration.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Obs!** En lista över filsystem som stöds för aktivitet vid åtkomst finns i [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)