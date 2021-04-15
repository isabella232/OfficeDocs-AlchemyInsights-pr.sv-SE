---
title: Ange eller ändra behörigheter för gemensamma mappar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789225"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="97827-102">Behörigheter och gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="97827-102">Permissions and Public Folders</span></span>

<span data-ttu-id="97827-103">Du kan ändra behörigheterna för dina gemensamma mappar med Outlook, Exchange admin center (EAC) eller PowerShell:</span><span class="sxs-lookup"><span data-stu-id="97827-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="97827-104">För Outlook instruktioner klickar [du här](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="97827-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="97827-105">Anvisningar för EAC finns i [den här](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) artikeln.</span><span class="sxs-lookup"><span data-stu-id="97827-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="97827-106">Anvisningar för Powershell finns i [den här artikeln](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) om hur du använder Add-PublicFolderClientPermission-kommandoleten.</span><span class="sxs-lookup"><span data-stu-id="97827-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="97827-107">Om du behöver anvisningar för att ansluta till Exchange Powershell klickar du [här](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="97827-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="97827-108">Om **externa användare inte kan skicka e-postmeddelanden** till en e-postaktiverad offentlig mapp, kan orsaken vara att den gemensamma mappen saknar de behörigheter som krävs för extern e-postleverans.</span><span class="sxs-lookup"><span data-stu-id="97827-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="97827-109">Du kan åtgärda detta med hjälp av [Outlook-instruktionerna här](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), eller PowerShell-instruktionerna [här](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="97827-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

