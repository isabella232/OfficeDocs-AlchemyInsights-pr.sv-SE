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
# <a name="configure-mim-sync-service"></a><span data-ttu-id="c8c97-102">Konfigurera MIM-synkroniseringstjänst</span><span class="sxs-lookup"><span data-stu-id="c8c97-102">Configure MIM Sync service</span></span>

<span data-ttu-id="c8c97-103">Synkroniseringstjänsten Microsoft Identity Manager (MIM) är en komponent i MIM.</span><span class="sxs-lookup"><span data-stu-id="c8c97-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="c8c97-104">Det är en centraliserad lokal tjänst som lagrar och integrerar information för organisationer som har flera lokala kataloger och databaser.</span><span class="sxs-lookup"><span data-stu-id="c8c97-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="c8c97-105">Du kan eventuellt lösa problemet med MIM-synkronisering om problemet åtgärdats i en nyligen uppdaterad MIM-uppdatering eller är ett av de andra problemen som nämns i avsnittet nedan.</span><span class="sxs-lookup"><span data-stu-id="c8c97-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="c8c97-106">**Rekommenderade steg**</span><span class="sxs-lookup"><span data-stu-id="c8c97-106">**Recommended steps**</span></span>

1. <span data-ttu-id="c8c97-107">Kontrollera att du använder den senaste uppdateringen av MIM-synkronisering och kontrollera viktig information om [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) för att avgöra om problemet har lösts i en uppdatering.</span><span class="sxs-lookup"><span data-stu-id="c8c97-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="c8c97-108">Om problemet beror på Generic LDAP-, Generic SQL-, Lotus Domino- eller Web Services-kopplingen bör du kontrollera att du använder en ny uppdatering av de [allmänna kopplingarna.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="c8c97-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="c8c97-109">Om ett MIM-synkroniseringskörning avslutas med ett fel tittar du i tabellen med [körfelkoder](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) för att fastställa möjliga orsaker.</span><span class="sxs-lookup"><span data-stu-id="c8c97-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="c8c97-110">Om körningen avbryts med undantag för **extension-dll-exception** klickar du på de orden för att öppna fönstret Egenskaper för kopplingsutrymmesobjekt och klickar på **Stack Trace...** för att se mer information om den underliggande orsaken, enligt beskrivningen i [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) </span><span class="sxs-lookup"><span data-stu-id="c8c97-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="c8c97-111">Om PCNS-komponenten (Password Change Notification Service) rapporterar felet **6025** i händelseloggen vid lösenordssynkronisering kan du läsa i guiden för felsökning av [PCNS-rapporteringsfel 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="c8c97-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="c8c97-112">Om fullständig synkronisering med FIM-tjänsthanteringsagenten går långsamt kan du kontrollera inställningen för att utöka automatiskt för TempDB, enligt beskrivningen i Felsökning – [långsam eller hängande fullständig synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) </span><span class="sxs-lookup"><span data-stu-id="c8c97-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="c8c97-113">Om du stöter på ett fel med stoppad server med tjänsten failed-creation-via-web-services med hjälp av FIM-tjänsthanteringsagenten kan du se [supportinformation: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) för en översikt över orsaker.</span><span class="sxs-lookup"><span data-stu-id="c8c97-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

