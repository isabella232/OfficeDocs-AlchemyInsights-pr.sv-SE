---
title: Ange eller ändra behörigheter för gemensamma mappar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36734687"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="5b895-102">Behörigheter och gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="5b895-102">Permissions and Public Folders</span></span>

<span data-ttu-id="5b895-103">Du kan ändra behörigheterna för dina gemensamma mappar med Outlook, Exchange Admin Center (UK) eller PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5b895-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="5b895-104">För Outlook-instruktioner, [Klicka här](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="5b895-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="5b895-105">För EAC, se [denna artikel](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) för instruktioner.</span><span class="sxs-lookup"><span data-stu-id="5b895-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="5b895-106">För PowerShell, referera till [den här artikeln](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) anvisningar om hur du använder den Lägg till PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="5b895-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="5b895-107">Om du behöver instruktioner för att ansluta till Exchange PowerShell, klicka [här](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="5b895-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="5b895-108">Om **externa användare inte kan skicka e-post till en e-postaktiverad offentlig mapp**, kan orsaken vara att den gemensamma mappen saknar behörigheter som krävs för extern e-postleverans.</span><span class="sxs-lookup"><span data-stu-id="5b895-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="5b895-109">Du kan åtgärda detta med hjälp av Outlook-instruktioner [här](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)eller PowerShell-instruktioner [här](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="5b895-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

