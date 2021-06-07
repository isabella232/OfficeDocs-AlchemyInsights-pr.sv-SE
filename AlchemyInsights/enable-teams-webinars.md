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
# <a name="enable-teams-webinars"></a><span data-ttu-id="f9d5b-102">Aktivera Teams webbseningar</span><span class="sxs-lookup"><span data-stu-id="f9d5b-102">Enable Teams Webinars</span></span>

<span data-ttu-id="f9d5b-103">Webbsnabs är aktiverade som standard.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-103">Webinars are enabled by default.</span></span> <span data-ttu-id="f9d5b-104">Med PowerShell-kommandon kan du hantera vem som kan schemalägga Teams registrera sig Teams Teams webbsendlar.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="f9d5b-105">Alla användare som kan skapa ett möte kan också skapa ett webbse-möte.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="f9d5b-106">Om du vill hantera vem som kan schemalägga Teams kan du använda *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="f9d5b-107">*WhoCanRegister är aktiverat och* inställt på Alla som **standard.**</span><span class="sxs-lookup"><span data-stu-id="f9d5b-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="f9d5b-108">Om du vill inaktivera mötesregistrering anger du *AllowMeetingRegistration till* **False**.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="f9d5b-109">Om du vill ändra de här inställningarna måste du [installera Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="f9d5b-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="f9d5b-110">Dessutom tillämpas mötesprinciper på Teams webbss webbseningar.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="f9d5b-111">Om anonym anslutning till exempel inaktiveras i mötesinställningarna kan anonyma användare inte ansluta till webbsswebbs.</span><span class="sxs-lookup"><span data-stu-id="f9d5b-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="f9d5b-112">Mer information om hur du konfigurerar vem som kan registrera sig för webbsenter finns i [Konfigurera vem som kan registrera sig för webbssalar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="f9d5b-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="f9d5b-113">Mer information om inställningar för Microsoft-listor finns i [Kontrollinställningar för Microsoft-listor.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="f9d5b-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>