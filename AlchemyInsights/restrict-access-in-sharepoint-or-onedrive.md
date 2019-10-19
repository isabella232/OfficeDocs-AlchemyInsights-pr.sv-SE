---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551469"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8d7e7-102">Begränsa åtkomsten i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="8d7e7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8d7e7-103">I SharePoint och OneDrive begränsar du åtkomsten till objekt som filer, mappar och listor genom att endast bevilja åtkomst till grupper eller personer som du vill ha åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="8d7e7-104">Som standard ärvs behörigheterna i SharePoint från högre upp i hierarkin.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="8d7e7-105">Så en fil ärver sina behörigheter från mappen, som ärver sina behörigheter från biblioteket, som ärver dess behörigheter från platsen.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="8d7e7-106">Du kan dela på en högre nivå (till exempel genom att dela en hel webbplats) och sedan bryta arv om du inte vill dela alla objekt på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="8d7e7-107">Men vi rekommenderar inte detta eftersom det gör att underhålla behörigheterna mer komplexa och förvirrande i framtiden.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="8d7e7-108">Det här kan du göra i stället:</span><span class="sxs-lookup"><span data-stu-id="8d7e7-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="8d7e7-109">Om du till exempel vill dela allt innehåll i en mapp med undantag för en fil i den, flyttar du filen till en ny plats som inte delas.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="8d7e7-110">Om du har två undermappar i en mapp och du vill dela en undermapp med grupperna A och B och endast tillåta grupp A-åtkomst till den andra undermappen, delar du den överordnade mappen med grupp A och lägger till grupp B i den första undermappen.</span><span class="sxs-lookup"><span data-stu-id="8d7e7-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="8d7e7-111">Sluta dela en fil eller mapp</span><span class="sxs-lookup"><span data-stu-id="8d7e7-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

