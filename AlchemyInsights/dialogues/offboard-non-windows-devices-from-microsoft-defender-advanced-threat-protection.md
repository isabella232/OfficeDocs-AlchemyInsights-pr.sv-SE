---
title: Offboard icke-Windows-enheter från Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695161"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard icke-Windows-enheter från Microsoft Defender Advanced Threat Protection (ATP)

Så här gör du:

1. Följ dokumentationen från tredje part för att koppla bort tredjepartslösningen från Microsoft Defender ATP.
2. Ta bort behörigheter för tredjepartslösningen från Azure Active Directory-klienten:

    1. Logga in på [Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Välj **Alla tjänster** Azure Active  >  **Directory** Enterprise  >  **Applications.**
    1. Välj det program du vill använda som offboard.
    1. Välj **Ta bort.**

Mer information finns i [Offboard-enheter som inte är Windows-enheter.](https://go.microsoft.com/fwlink/?linkid=2143630)
