---
title: Hantera registrering för webbsswebb
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794145"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="c37ae-102">Hantera registrering för webbsswebb</span><span class="sxs-lookup"><span data-stu-id="c37ae-102">Manage webinar registration</span></span>

<span data-ttu-id="c37ae-103">Du hanterar vem som kan registrera sig för Teams-webbssyssor med hjälp Teams Powershell-kommandon.</span><span class="sxs-lookup"><span data-stu-id="c37ae-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="c37ae-104">Information om hur du Teams Powershell finns [i Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="c37ae-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="c37ae-105">*WhoCanRegister är aktiverat och* inställt på **EveryoneInCompany som standard.**</span><span class="sxs-lookup"><span data-stu-id="c37ae-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="c37ae-106">Om du vill tillåta att alla, även anonyma användare, registrerar sig måste du ställa in mötespolicyn på **Alla** med powershell-kommandot:</span><span class="sxs-lookup"><span data-stu-id="c37ae-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="c37ae-107">**Obs!** Om anonym anslutning har inaktiverats i mötesinställningarna kan anonyma användare inte ansluta till webbss webbseningar.</span><span class="sxs-lookup"><span data-stu-id="c37ae-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="c37ae-108">Mer information och hur du aktiverar den här inställningen finns [i Hantera mötesinställningar i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="c37ae-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="c37ae-109">Om du vill inaktivera mötesregistrering anger du *AllowMeetingRegistration till* **False**.</span><span class="sxs-lookup"><span data-stu-id="c37ae-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="c37ae-110">Mer information om hur du konfigurerar vem som kan registrera sig för webbsenter finns i [Konfigurera vem som kan registrera sig för webbssalar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="c37ae-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="c37ae-111">Mer information om inställningar för Microsoft-listor finns i [Kontrollinställningar för Microsoft-listor.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="c37ae-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
