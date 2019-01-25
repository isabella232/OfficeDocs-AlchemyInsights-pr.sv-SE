---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492215"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="046ff-102">Begränsa åtkomsten i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="046ff-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="046ff-p101">I SharePoint och OneDrive kan begränsa du åtkomsten till objekt som filer, mappar och listor genom att bevilja åtkomst till grupper eller användare som du vill ska ha åtkomst. Som standard ärvs behörigheterna i SharePoint från högre upp i hierarkin. Så ärver en fil dess behörigheter från mappen som har ärvt sina rättigheter från biblioteket som ärver dess behörighet från webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="046ff-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="046ff-p102">Du kan dela på en högre nivå (t ex genom att dela en hel webbplats) och sedan bryta arvet om du inte vill dela alla objekt på webbplatsen. Men rekommenderar vi inte detta eftersom det gör att underhålla behörigheter mer komplexa och förvirrande i framtiden. Det här är vad du kan göra i stället:</span><span class="sxs-lookup"><span data-stu-id="046ff-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="046ff-109">Om du till exempel vill dela hela innehållet i en mapp med undantag för en fil i den, kan du flytta filen till en ny plats som inte är delad.</span><span class="sxs-lookup"><span data-stu-id="046ff-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="046ff-110">Om du har två undermappar i en mapp och du vill dela en undermapp med grupperna A och B och tillåter endast grupp A åtkomsten till undermappen andra, dela den överordnade mappen med grupp A och Lägg till grupp B i den första undermappen.</span><span class="sxs-lookup"><span data-stu-id="046ff-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="046ff-111">Sluta dela en fil eller mapp</span><span class="sxs-lookup"><span data-stu-id="046ff-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

