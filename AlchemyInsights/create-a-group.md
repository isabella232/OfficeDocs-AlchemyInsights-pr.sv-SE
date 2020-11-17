---
title: Skapa en grupp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089177"
---
# <a name="create-a-group"></a><span data-ttu-id="e9889-102">Skapa en grupp</span><span class="sxs-lookup"><span data-stu-id="e9889-102">Create a group</span></span>

<span data-ttu-id="e9889-103">I det här avsnittet beskrivs hur du skapar grupper.</span><span class="sxs-lookup"><span data-stu-id="e9889-103">This topic describes group creation.</span></span>

<span data-ttu-id="e9889-104">**Behörighet att skapa en grupp**</span><span class="sxs-lookup"><span data-stu-id="e9889-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="e9889-105">Se till att du har behörighet att skapa en ny grupp.</span><span class="sxs-lookup"><span data-stu-id="e9889-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="e9889-106">Globala administratörer kan inaktivera skapande av grupper i Azure Portal eller åtkomst panelen.</span><span class="sxs-lookup"><span data-stu-id="e9889-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="e9889-107">Du kan behöva en administratör för att skapa den nya gruppen åt dig, eller ge dig lämpliga behörigheter.</span><span class="sxs-lookup"><span data-stu-id="e9889-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="e9889-108">**Hantera behörigheter för grupp skapande**</span><span class="sxs-lookup"><span data-stu-id="e9889-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="e9889-109">Globala administratörer kan hantera behörigheter för grupp skapande (av säkerhetsrelaterade skäl) eller Office 365-grupper som har skapats i Azure-portalen eller åtkomst panelen genom att välja "användare kan skapa säkerhets grupper i Azure-portaler" eller "användare kan skapa Office 365-grupper i Azure portaler" i **alla grupper**  >  **Allmänt (inställningar)**.</span><span class="sxs-lookup"><span data-stu-id="e9889-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="e9889-110">Du kan också begränsa grupp skapande för att välja en grupp användare om du har en Azure Active Directory P1 Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="e9889-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="e9889-111">**Inaktiverar välkomst meddelande för nya Office 365-gruppmedlemmar**</span><span class="sxs-lookup"><span data-stu-id="e9889-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="e9889-112">Välkomst meddelandet som skickas till användare som har lagts till i Office 365 grupper kan inaktive ras genom att ange **UnifiedGroupWelcomeMessageEnabled** till falskt i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e9889-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="e9889-113">Lär dig mer om den [här inställningen.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="e9889-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

