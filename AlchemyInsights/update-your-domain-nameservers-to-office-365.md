---
title: Uppdatera dina domännamnservrar så att de pekar på Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734929"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="b276e-102">Uppdatera dina domännamnservrar så att de pekar på Microsoft</span><span class="sxs-lookup"><span data-stu-id="b276e-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="b276e-103">Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.</span><span class="sxs-lookup"><span data-stu-id="b276e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="b276e-104">För att konfigurera din domän hos Microsoft måste namnservrar hos din registrator uppdateras.</span><span class="sxs-lookup"><span data-stu-id="b276e-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="b276e-105">Skapa eller redigera dina namnserverposter hos din domänregistrator.</span><span class="sxs-lookup"><span data-stu-id="b276e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="b276e-106">Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.</span><span class="sxs-lookup"><span data-stu-id="b276e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="b276e-107">Skapa eller redigera två namnserverposterna så att de matchar följande värden:</span><span class="sxs-lookup"><span data-stu-id="b276e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="b276e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b276e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="b276e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b276e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="b276e-110">Spara ändringar.</span><span class="sxs-lookup"><span data-stu-id="b276e-110">Save changes.</span></span>

<span data-ttu-id="b276e-111">Detaljerade anvisningar finns i den här artikeln: [ändra namnservrar för att konfigurera Microsoft 365 med valfri domän registrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="b276e-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  