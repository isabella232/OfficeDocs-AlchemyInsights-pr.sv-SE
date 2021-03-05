---
title: Konfigurera MIM-synkroniseringstjänst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482896"
---
# <a name="configure-mim-sync-service"></a>Konfigurera MIM-synkroniseringstjänst

Synkroniseringstjänsten Microsoft Identity Manager (MIM) är en komponent i MIM. Det är en centraliserad lokal tjänst som lagrar och integrerar information för organisationer som har flera lokala kataloger och databaser. Du kan eventuellt lösa problemet med MIM-synkronisering om problemet åtgärdats i en nyligen uppdaterad MIM-uppdatering eller är ett av de andra problemen som nämns i avsnittet nedan.

**Rekommenderade steg**

1. Kontrollera att du använder den senaste uppdateringen av MIM-synkronisering och kontrollera viktig information om [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) för att avgöra om problemet har lösts i en uppdatering.
2. Om problemet beror på Generic LDAP-, Generic SQL-, Lotus Domino- eller Web Services-kopplingen bör du kontrollera att du använder en ny uppdatering av de [allmänna kopplingarna.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Om ett MIM-synkroniseringskörning avslutas med ett fel tittar du i tabellen med [körfelkoder](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) för att fastställa möjliga orsaker.
4. Om körningen avbryts med undantag för **extension-dll-exception** klickar du på de orden för att öppna fönstret Egenskaper för kopplingsutrymmesobjekt och klickar på **Stack Trace...** för att se mer information om den underliggande orsaken, enligt beskrivningen i [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 
5. Om PCNS-komponenten (Password Change Notification Service) rapporterar felet **6025** i händelseloggen vid lösenordssynkronisering kan du läsa i guiden för felsökning av [PCNS-rapporteringsfel 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Om fullständig synkronisering med FIM-tjänsthanteringsagenten går långsamt kan du kontrollera inställningen för att utöka automatiskt för TempDB, enligt beskrivningen i Felsökning – [långsam eller hängande fullständig synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) 
7. Om du stöter på ett fel med stoppad server med tjänsten failed-creation-via-web-services med hjälp av FIM-tjänsthanteringsagenten kan du se [supportinformation: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) för en översikt över orsaker.

