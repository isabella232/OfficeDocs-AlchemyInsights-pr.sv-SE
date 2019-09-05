---
title: Behörighetsproblem vid migrering
ms.author: pebaum
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 33e605ff3019f52bbd0be876d485ff389b260a44
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752640"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="84f72-102">Användarprofil och Fotosynkronisering</span><span class="sxs-lookup"><span data-stu-id="84f72-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="84f72-103">**Synkronisering av profilfoto** -användare kan märka att deras profilfoto inte synkroniseras till SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84f72-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="84f72-104">Eller så kan de ha försökt uppdatera sin profilbild och fotot visas fortfarande som det gamla fotot.</span><span class="sxs-lookup"><span data-stu-id="84f72-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="84f72-105">För att säkerställa att profilfotot visas som förväntat måste användaren initiera en Fotosynkronisering.</span><span class="sxs-lookup"><span data-stu-id="84f72-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="84f72-106">Mer information om synkroniseringsprocessen för foto finns [i information om synkronisering av profilbilder i Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="84f72-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="84f72-107">**Profilsynkronisering** -den tid som krävs för att slutföra en profilsynkronisering beror på antalet ändringar (arbete) som AD-importjobbet måste bearbeta.</span><span class="sxs-lookup"><span data-stu-id="84f72-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="84f72-108">Om det finns många ändringar, har det tidsinställda jobbet en hel del arbete att göra, och det tar längre tid för ändringarna återspeglas i användarprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="84f72-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="84f72-109">Om det tidsinställda jobbet har en liten mängd arbete att göra, kommer ändringarna återspeglas i användarprofilprogrammet mycket snabbare.</span><span class="sxs-lookup"><span data-stu-id="84f72-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="84f72-110">Mer information om synkroniseringsprocessen för profiler finns [i information om synkronisering av användarprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="84f72-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="84f72-111">**Uppdatera profil i Office Delve** -Delve användare kan hantera sin Office 365-profil.</span><span class="sxs-lookup"><span data-stu-id="84f72-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="84f72-112">Mer information finns [i Visa och uppdatera din profil i Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="84f72-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

