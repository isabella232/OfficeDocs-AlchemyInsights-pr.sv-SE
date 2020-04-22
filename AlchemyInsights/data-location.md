---
title: Plats för data
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655300"
---
# <a name="data-location"></a><span data-ttu-id="7857a-102">Plats för data</span><span class="sxs-lookup"><span data-stu-id="7857a-102">Data location</span></span>

<span data-ttu-id="7857a-103">Du kan visa platsen för din klient i administrationscentret eller genom att ansluta till Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7857a-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="7857a-104">**Administrationscenter:**</span><span class="sxs-lookup"><span data-stu-id="7857a-104">**Admin center:**</span></span>
1. <span data-ttu-id="7857a-105">Logga in på [administrationscentret](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="7857a-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="7857a-106">Välj profil **för inställningar** > **organisation**.</span><span class="sxs-lookup"><span data-stu-id="7857a-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="7857a-107">Under **Dataplats**väljer du **Visa information**.</span><span class="sxs-lookup"><span data-stu-id="7857a-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="7857a-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="7857a-108">**PowerShell:**</span></span>
1. <span data-ttu-id="7857a-109">Anslut till Exchange Online med Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7857a-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="7857a-110">Kör [cmdleten Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) för att visa en lista över klientens egenskaper.</span><span class="sxs-lookup"><span data-stu-id="7857a-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="7857a-111">Titta på OrganisationenId egendom.</span><span class="sxs-lookup"><span data-stu-id="7857a-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="7857a-112">När du har dataplatsen för EXO och SPO kan du bestämma vilken dataplats för andra tjänster du kan använda från [där dina data finns](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="7857a-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>