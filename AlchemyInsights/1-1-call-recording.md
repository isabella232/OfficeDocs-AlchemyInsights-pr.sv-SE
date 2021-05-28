---
title: Inspelning av 1:1-samtal
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696976"
---
# <a name="11-call-recording"></a>Inspelning av 1:1-samtal

Om **knappen Starta** inspelning är nedtonad under ett nödsamtal måste du ändra principinställningarna för den påverkade användaren.   

Med början den 31 maj 2021 börjar vi framtvinga en ny Teams *AllowCloudRecordingForCalls.* Innan den här ändringen kontrolleras inspelning av 1:1-samtal av *AllowCloudRecording* Teams mötespolicyn. Den här ändringen har dokumenterats i inlägget i meddelandecentret: [(Uppdaterad) 1:1 Inledningen till inspelningspolicyn för samtal.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   alternativet för samtalsprincip är **$False** som standard. Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd.  

Om du vill aktivera samtalsinspelning för alla användare i 1:1-samtal använder Teams PowerShell för att köra följande cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Du kan också skapa en ny princip och ange **-AllowCloudRecordingForCalls** **$true** tilldela den principen till användarna. 

Mer information finns i [principkontroller för samtalsinspelning är (nästan!) Här](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
