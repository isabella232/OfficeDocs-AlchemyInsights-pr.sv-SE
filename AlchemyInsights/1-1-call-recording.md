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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886157"
---
# <a name="11-call-recording"></a>Inspelning av 1:1-samtal

Om **knappen Starta** inspelning är nedtonad under ett nödsamtal måste du ändra principinställningarna för den påverkade användaren. Kontrollera principinställningen genom att köra Diagnostik för den påverkade användaren genom att skriva **Diag: Teams 1:1-samtalsinspelning** ovan.     

Med början den 31 maj 2021 börjar vi framtvinga en ny Teams *AllowCloudRecordingForCalls.* Innan den här ändringen kontrolleras inspelning av 1:1-samtal av *AllowCloudRecording* Teams mötespolicyn. Den här ändringen har dokumenterats i inlägget i meddelandecentret: [(Uppdaterad) 1:1 Inledningen till inspelningspolicyn för samtal.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   alternativet för samtalsprincip är **$False** som standard. Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd.  

Om du vill aktivera samtalsinspelning för alla användare i 1:1-samtal [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) för att köra följande cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativt kan du skapa en ny princip och ange **-AllowCloudRecordingForCalls** **$true** tilldela den principen till dina användare. 

Mer information finns i [principkontroller för samtalsinspelning är (nästan!) Här](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
