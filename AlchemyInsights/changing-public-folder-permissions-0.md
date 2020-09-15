---
title: Ändra behörigheter för en gemensam mapp
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714265"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="34e90-102">Ändra behörigheter för en gemensam mapp</span><span class="sxs-lookup"><span data-stu-id="34e90-102">Changing public folder permissions</span></span>

<span data-ttu-id="34e90-103">Behörigheter för den offentliga mappen kan ändras av användare och administratörer i Outlook.</span><span class="sxs-lookup"><span data-stu-id="34e90-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="34e90-104">Administratörer kan även kontrol lera behörigheter från administrations centret för Exchange (UK) genom att göra följande:</span><span class="sxs-lookup"><span data-stu-id="34e90-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="34e90-105">Öppna administrations centret för Microsoft 365 och gå **till** \> **Exchange**-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="34e90-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="34e90-106">Välj **gemensamma mappar**.</span><span class="sxs-lookup"><span data-stu-id="34e90-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="34e90-107">Därifrån kan du ändra behörigheterna för enskilda gemensamma mappar genom att tilldela säkerhets grupper till behörigheter.</span><span class="sxs-lookup"><span data-stu-id="34e90-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="34e90-108">För att slutanvändaren ska kunna ändra behörigheter för en gemensam mapp måste användaren ha ägar rättigheter för mappen.</span><span class="sxs-lookup"><span data-stu-id="34e90-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="34e90-109">Följ anvisningarna i artikeln om [hur du kan diagnostisera och åtgärda problem med den offentliga mappen](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) för att felsöka problem med den offentliga mappen.</span><span class="sxs-lookup"><span data-stu-id="34e90-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="34e90-110">**Obs!** det finns flera kända problem som du kan stöta på när du försöker ändra behörigheter för gemensamma mappar.</span><span class="sxs-lookup"><span data-stu-id="34e90-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="34e90-111">Mer information finns i följande artiklar.</span><span class="sxs-lookup"><span data-stu-id="34e90-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="34e90-112">Det går inte att tillämpa behörigheter för undermappar i gemensamma mappar i UK</span><span class="sxs-lookup"><span data-stu-id="34e90-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="34e90-113">Felet "post lådan hittas inte i den lokala skogen" när du öppnar gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="34e90-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
