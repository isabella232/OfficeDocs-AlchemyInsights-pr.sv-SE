---
title: Återställ borttagen post låda
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728089"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="a8b14-102">Återställa en borttagen post låda</span><span class="sxs-lookup"><span data-stu-id="a8b14-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="a8b14-103">När en användare förlorar en Exchange Online-licens sparas post lådan i 30 dagar och kan återställas genom att helt enkelt tilldela licensen till användaren.</span><span class="sxs-lookup"><span data-stu-id="a8b14-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="a8b14-104">*Detta fungerar bara inom 30 dagar.*</span><span class="sxs-lookup"><span data-stu-id="a8b14-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="a8b14-105">Gå till sidan **användare** \> **aktiva användare** i administrations centret för Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a8b14-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="a8b14-106">Välj den användare du vill.</span><span class="sxs-lookup"><span data-stu-id="a8b14-106">Select the user in question.</span></span>

2. <span data-ttu-id="a8b14-107">På fliken **licenser och appar** tilldelar du Exchange Online-licensen och väljer **Spara ändringar**.</span><span class="sxs-lookup"><span data-stu-id="a8b14-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="a8b14-108">Om du försöker återställa en delad post låda kan den också avsättas i 30 dagar.</span><span class="sxs-lookup"><span data-stu-id="a8b14-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="a8b14-109">Du hittar dem under **användares** \> **borttagna användare**; delade post lådor kräver ingen licens.</span><span class="sxs-lookup"><span data-stu-id="a8b14-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="a8b14-110">Om du vill återställa en borttagen användare kan du läsa [återställa en användare](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a8b14-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  