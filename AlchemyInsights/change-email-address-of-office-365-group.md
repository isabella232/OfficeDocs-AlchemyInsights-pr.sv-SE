---
title: Ändra e-postadress för en Microsoft 365-grupp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580675"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="c5d53-102">Ändra e-postadress för en Microsoft 365-grupp</span><span class="sxs-lookup"><span data-stu-id="c5d53-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="c5d53-103">Du kan ändra e-postadressen för en Microsoft 365-grupp med hjälp av administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="c5d53-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c5d53-104">Välj bara gruppen och välj @edit e-postadress.</span><span class="sxs-lookup"><span data-stu-id="c5d53-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c5d53-105">Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp:</span><span class="sxs-lookup"><span data-stu-id="c5d53-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="c5d53-106">Ange unifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c5d53-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c5d53-107">Exempel:</span><span class="sxs-lookup"><span data-stu-id="c5d53-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
