---
title: Data plats
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627864"
---
# <a name="data-location"></a><span data-ttu-id="26990-102">Data plats</span><span class="sxs-lookup"><span data-stu-id="26990-102">Data location</span></span>

<span data-ttu-id="26990-103">Du kan visa platsen för din Office 365-klient i administratörscenter eller genom att ansluta till Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="26990-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="26990-104">**Admin Center:**</span><span class="sxs-lookup"><span data-stu-id="26990-104">**Admin center:**</span></span>
1. <span data-ttu-id="26990-105">Logga in på [administratörscenter](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="26990-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="26990-106">Välj **Inställningar** > **organisations profil**.</span><span class="sxs-lookup"><span data-stu-id="26990-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="26990-107">Under **data plats**väljer du **Visa information**.</span><span class="sxs-lookup"><span data-stu-id="26990-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="26990-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="26990-108">**PowerShell:**</span></span>
1. <span data-ttu-id="26990-109">Ansluta till Exchange Online med hjälp av Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="26990-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="26990-110">Kör cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) om du vill visa en lista över klientens egenskaper.</span><span class="sxs-lookup"><span data-stu-id="26990-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="26990-111">Titta på egenskapen OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="26990-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="26990-112">När du har data platsen för EXO och SPO kan du bestämma data platsen för andra tjänster som du kan använda [varifrån dina data finns](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="26990-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>