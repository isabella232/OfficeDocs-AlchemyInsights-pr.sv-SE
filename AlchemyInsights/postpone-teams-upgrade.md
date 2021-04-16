---
title: Skjuta upp uppgradering av Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801249"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="a6767-102">Så här skjuter du upp uppgraderingen av Microsoft-drivna Teams</span><span class="sxs-lookup"><span data-stu-id="a6767-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="a6767-103">**Viktigt:** Vi kan hjälpa dig att lösa detta med hjälp av ett supportdiagnostik, men det verkar som att du inte använder det nya administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="a6767-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="a6767-104">Om du vill använda det nya administrationscentret drar du reglaget uppe till höger, där **det står nytt administrationscenter** till höger.</span><span class="sxs-lookup"><span data-stu-id="a6767-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="a6767-105">Med hjälp av nya administrationscentret klickar du på widgeten Behöver du **hjälp?,** skriver "Skjut upp teams-uppgradering" och följer sedan anvisningarna för att köra diagnostikverktyget.</span><span class="sxs-lookup"><span data-stu-id="a6767-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="a6767-106">Om du har fått information om en automatiserad Microsoft-uppgradering från Skype för företag till Microsoft Teams och du vill skjuta upp den automatiska uppgraderingen till ett senare datum  kan din globala administratör logga in på [Teams](https://admin.teams.microsoft.com/dashboard) administrationsportal och när du har valt knappen Uppdatera **status** under Microsoft Teams-uppgradering väljer du knappen Skjut upp.</span><span class="sxs-lookup"><span data-stu-id="a6767-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="a6767-107">Uppdatera sidan på administrationsportalen för Teams om du vill se det nya datumet för din klientorganisations automatiska uppgradering till Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a6767-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="a6767-108">**Obs!** Knappen **Skjut** upp är bara tillgänglig om du har fått meddelandet i meddelandecentret om den automatiska uppgraderingen.</span><span class="sxs-lookup"><span data-stu-id="a6767-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="a6767-109">Globala administratörer kan även köra [Get-CsTeamsUpgradeStatus om](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) du vill veta mer om deras aktuella uppgraderingsstatus.</span><span class="sxs-lookup"><span data-stu-id="a6767-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
