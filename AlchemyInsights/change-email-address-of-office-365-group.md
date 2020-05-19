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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283262"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c50b3-102">Ändra e-postadress för en Microsoft 365-grupp</span><span class="sxs-lookup"><span data-stu-id="c50b3-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c50b3-103">Du kan ändra e-postadressen för en Microsoft 365-grupp med hjälp av administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="c50b3-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c50b3-104">Välj bara gruppen och välj @edit e-postadress.</span><span class="sxs-lookup"><span data-stu-id="c50b3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c50b3-105">Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp:</span><span class="sxs-lookup"><span data-stu-id="c50b3-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c50b3-106">Ange unifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c50b3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c50b3-107">Exempel:</span><span class="sxs-lookup"><span data-stu-id="c50b3-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
