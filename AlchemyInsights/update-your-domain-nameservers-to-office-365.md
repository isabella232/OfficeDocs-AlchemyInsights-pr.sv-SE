---
title: Uppdatera dina domännamnservrar till Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742205"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="0ea66-102">Uppdatera dina domännamnservrar till Office 365</span><span class="sxs-lookup"><span data-stu-id="0ea66-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="0ea66-103">Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.</span><span class="sxs-lookup"><span data-stu-id="0ea66-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="0ea66-p101">Om du vill konfigurera din domän i Office 365 måste dina namnservrar hos registratorn uppdateras. Skapa eller redigera dina namnserverposter hos din domänregistrator.</span><span class="sxs-lookup"><span data-stu-id="0ea66-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="0ea66-106">Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.</span><span class="sxs-lookup"><span data-stu-id="0ea66-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="0ea66-107">Skapa eller redigera två namnserverposterna så att de matchar följande värden:</span><span class="sxs-lookup"><span data-stu-id="0ea66-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="0ea66-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0ea66-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="0ea66-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0ea66-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="0ea66-110">Spara ändringar.</span><span class="sxs-lookup"><span data-stu-id="0ea66-110">Save changes.</span></span>

<span data-ttu-id="0ea66-111">Du kan också hitta detaljerade instruktioner i den här artikeln: [Ändra namnservrar för att konfigurera Office 365 med valfri domänregistrator](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="0ea66-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  