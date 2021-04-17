---
title: Skapa en grupp
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816390"
---
# <a name="create-a-group"></a><span data-ttu-id="a4621-102">Skapa en grupp</span><span class="sxs-lookup"><span data-stu-id="a4621-102">Create a group</span></span>

<span data-ttu-id="a4621-103">I det här avsnittet beskrivs hur du skapar grupper.</span><span class="sxs-lookup"><span data-stu-id="a4621-103">This topic describes group creation.</span></span>

<span data-ttu-id="a4621-104">**Behörighet att skapa en grupp**</span><span class="sxs-lookup"><span data-stu-id="a4621-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="a4621-105">Se till att du har behörighet att skapa en ny grupp.</span><span class="sxs-lookup"><span data-stu-id="a4621-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="a4621-106">Globala administratörer kan inaktivera skapande av grupper i Azure-portalen eller åtkomstpanelen.</span><span class="sxs-lookup"><span data-stu-id="a4621-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="a4621-107">Du kan behöva en administratör för att skapa den nya gruppen åt dig eller ge dig rätt behörigheter.</span><span class="sxs-lookup"><span data-stu-id="a4621-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="a4621-108">**Hantera behörigheter för att skapa grupper**</span><span class="sxs-lookup"><span data-stu-id="a4621-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="a4621-109">Globala administratörer kan hantera behörigheter för att skapa grupper (av säkerhetsrelaterade orsaker) eller Office 365-grupper som skapats i Azure-portalen eller åtkomstpanelen genom att välja alternativen "Användare kan skapa säkerhetsgrupper i Azure-portaler" eller "Användare kan skapa Office 365-grupper i Azure-portaler" i Alla grupper Allmänt  >  **(Inställningar)**.</span><span class="sxs-lookup"><span data-stu-id="a4621-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="a4621-110">Du kan också begränsa möjligheten att skapa grupper om du vill välja en grupp användare om du har en Azure Active Directory P1 Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="a4621-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="a4621-111">**Inaktivera välkomstmeddelande för nya medlemmar i Office 365-grupper**</span><span class="sxs-lookup"><span data-stu-id="a4621-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="a4621-112">Välkomstmeddelandet som skickas till användare som läggs till i Office 365-grupper kan inaktiveras genom att ställa in **UnifiedGroupWelcomeMessageEnabled** till False i Powershell.</span><span class="sxs-lookup"><span data-stu-id="a4621-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="a4621-113">Läs mer om den här inställningen [här](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a4621-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

