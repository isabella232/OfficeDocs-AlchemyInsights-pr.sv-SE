---
title: Mappen skicka som e-postaktive rad EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462074"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="a070a-102">Skicka som e-postaktiverad gemensam mapp</span><span class="sxs-lookup"><span data-stu-id="a070a-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="a070a-103">I följande exempel tilldelas "Send As"-behörigheter för den e-postaktiverade gemensamma mappen NewPF1 till användarens Jason.</span><span class="sxs-lookup"><span data-stu-id="a070a-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="a070a-104">Add-RecipientPermission-Identity ' NewPF1 '-förvaltaren "Jason"-AccessRights ' sende '</span><span class="sxs-lookup"><span data-stu-id="a070a-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="a070a-105">Detaljerad information om syntax och parametrar finns i [tilldela behörigheter för att skicka som eller skicka för e-postaktiverade gemensamma mappar](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="a070a-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

