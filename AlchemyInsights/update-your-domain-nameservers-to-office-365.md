---
title: Uppdatera dina domännamnservrar så att de pekar på Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510302"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="3452f-102">Uppdatera dina domännamnservrar så att de pekar på Microsoft</span><span class="sxs-lookup"><span data-stu-id="3452f-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="3452f-103">Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.</span><span class="sxs-lookup"><span data-stu-id="3452f-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3452f-104">Om du vill konfigurera domänen med Microsoft måste namnservrarna på din registrator uppdateras.</span><span class="sxs-lookup"><span data-stu-id="3452f-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="3452f-105">Skapa eller redigera dina namnserverposter hos din domänregistrator.</span><span class="sxs-lookup"><span data-stu-id="3452f-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3452f-106">Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.</span><span class="sxs-lookup"><span data-stu-id="3452f-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="3452f-107">Skapa eller redigera två namnserverposterna så att de matchar följande värden:</span><span class="sxs-lookup"><span data-stu-id="3452f-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3452f-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3452f-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3452f-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3452f-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3452f-110">Spara ändringar.</span><span class="sxs-lookup"><span data-stu-id="3452f-110">Save changes.</span></span>

<span data-ttu-id="3452f-111">Du kan också hitta detaljerade instruktioner i den här artikeln: [Ändra namnservrar för att konfigurera Microsoft 365 med alla domänregistratorer](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="3452f-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  