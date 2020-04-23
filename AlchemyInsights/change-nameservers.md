---
title: Ändra namnservrar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706773"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="82280-102">Uppdatera dina domännamnservrar så att de pekar på Microsoft</span><span class="sxs-lookup"><span data-stu-id="82280-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="82280-103">Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.</span><span class="sxs-lookup"><span data-stu-id="82280-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="82280-p101">Om du vill konfigurera din domän i Microsoft 365 måste du uppdatera dina namnservrar hos registratorn. Skapa eller redigera dina namnserverposter hos din domänregistrator.</span><span class="sxs-lookup"><span data-stu-id="82280-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="82280-106">Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.</span><span class="sxs-lookup"><span data-stu-id="82280-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="82280-107">Skapa eller redigera två namnserverposterna så att de matchar följande värden:</span><span class="sxs-lookup"><span data-stu-id="82280-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="82280-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="82280-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="82280-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="82280-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="82280-110">Spara ändringar.</span><span class="sxs-lookup"><span data-stu-id="82280-110">Save changes.</span></span>

<span data-ttu-id="82280-111">Du kan också hitta detaljerade instruktioner i den här artikeln: [Ändra namnservrar hos valfri domänregistrator](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="82280-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  