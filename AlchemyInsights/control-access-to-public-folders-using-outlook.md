---
title: Kontrollera åtkomst till gemensamma mappar med Hjälp av Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816758"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="c37ae-102">Kontrollera åtkomst till gemensamma mappar med Hjälp av Outlook</span><span class="sxs-lookup"><span data-stu-id="c37ae-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="c37ae-103">Så här styr du vilka användare som kan komma åt gemensamma mappar i Outlook:</span><span class="sxs-lookup"><span data-stu-id="c37ae-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="c37ae-104">Använd `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="c37ae-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="c37ae-105">$true: Tillåta användare åtkomst till gemensamma mappar i Outlook</span><span class="sxs-lookup"><span data-stu-id="c37ae-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="c37ae-106">$false: Förhindra att användare kommer åt gemensamma mappar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="c37ae-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="c37ae-107">Det här är standardvärdet.</span><span class="sxs-lookup"><span data-stu-id="c37ae-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="c37ae-108">Obs! Den här proceduren kan bara styra anslutningar med Outlook för Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="c37ae-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="c37ae-109">Användare kan fortsätta komma åt gemensamma mappar med hjälp av OWA eller Outlook för Mac.</span><span class="sxs-lookup"><span data-stu-id="c37ae-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="c37ae-110">Mer information finns i [Kontrollerade anslutningar till gemensamma mappar i Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="c37ae-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
