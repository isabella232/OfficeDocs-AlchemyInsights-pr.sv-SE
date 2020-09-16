---
title: Begränsa åtkomst i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720700"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f37f9-102">Begränsa åtkomst i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="f37f9-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f37f9-103">I SharePoint och OneDrive kan du begränsa åtkomsten till objekt som filer, mappar och listor genom att endast bevilja åtkomst till grupper eller personer som du vill ha åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="f37f9-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f37f9-104">Som standard ärvs behörigheter i SharePoint från högre upp i hierarkin.</span><span class="sxs-lookup"><span data-stu-id="f37f9-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f37f9-105">En fil ärver behörigheterna från mappen, som ärver dess behörigheter från biblioteket, som ärver dess behörigheter från webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="f37f9-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f37f9-106">Du kan dela på en högre nivå (till exempel genom att dela en hel webbplats) och sedan bryta arvet om du inte vill dela alla objekt på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="f37f9-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f37f9-107">Vi rekommenderar emellertid inte detta eftersom det gör det lättare att bevara dina behörigheter.</span><span class="sxs-lookup"><span data-stu-id="f37f9-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f37f9-108">Det här kan du göra i stället:</span><span class="sxs-lookup"><span data-stu-id="f37f9-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f37f9-109">Om du till exempel vill dela hela innehållet i en mapp, förutom en fil i den, kan du flytta filen till en ny plats som inte är delad.</span><span class="sxs-lookup"><span data-stu-id="f37f9-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f37f9-110">Om du har två undermappar i en mapp och vill dela en undermapp med grupp A och B och bara tillåta grupp åtkomst till den andra undermappen delar du den överordnade mappen med grupp A och lägger till grupp B i den första undermappen.</span><span class="sxs-lookup"><span data-stu-id="f37f9-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f37f9-111">Sluta dela en fil eller mapp </span><span class="sxs-lookup"><span data-stu-id="f37f9-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

