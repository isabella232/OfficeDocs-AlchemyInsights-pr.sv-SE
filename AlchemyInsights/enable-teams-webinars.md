---
title: Aktivera Teams webbseningar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794038"
---
# <a name="enable-teams-webinars"></a>Aktivera Teams webbseningar

Webbsnabs är aktiverade som standard. Med PowerShell-kommandon kan du hantera vem som kan schemalägga Teams registrera sig Teams Teams webbsendlar.

- Alla användare som kan skapa ett möte kan också skapa ett webbse-möte. Om du vill hantera vem som kan schemalägga Teams kan du använda *AllowMeetingRegistration*. 
- *WhoCanRegister är aktiverat och* inställt på Alla som **standard.** Om du vill inaktivera mötesregistrering anger du *AllowMeetingRegistration till* **False**.

Om du vill ändra de här inställningarna måste du [installera Teams PowerShell.](/microsoftteams/teams-powershell-install) Dessutom tillämpas mötesprinciper på Teams webbss webbseningar. Om anonym anslutning till exempel inaktiveras i mötesinställningarna kan anonyma användare inte ansluta till webbsswebbs.

Mer information om hur du konfigurerar vem som kan registrera sig för webbsenter finns i [Konfigurera vem som kan registrera sig för webbssalar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Mer information om inställningar för Microsoft-listor finns i [Kontrollinställningar för Microsoft-listor.](/sharepoint/control-lists)