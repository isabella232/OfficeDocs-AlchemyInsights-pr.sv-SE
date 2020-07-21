---
title: Flera användare ser inte tillägg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198243"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="a9f5b-102">Flera användare ser inte tillägg i Outlook</span><span class="sxs-lookup"><span data-stu-id="a9f5b-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="a9f5b-103">Om du testar Outlook-tillägg och ingen visas, som ett första felsökningssteg, använder du **Get-OrganizationConfig** PowerShell-cmdlet för att fråga parametern _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="a9f5b-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="a9f5b-104">Om frågan returnerar ett värde i **False**anger du den här parametern till **True** med hjälp av **cmdlet Set-OrganizationConfig,** så att tillägg visas som förväntat.</span><span class="sxs-lookup"><span data-stu-id="a9f5b-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="a9f5b-105">Vi rekommenderar inte att parametern _AppsForOfficeEnabled_ är inställd på **False**.</span><span class="sxs-lookup"><span data-stu-id="a9f5b-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="a9f5b-106">Värdet **False** åsidosätter alla ovanstående inställningar för administratörs- och användarroll och förhindrar att nya appar aktiveras av alla användare i organisationen.</span><span class="sxs-lookup"><span data-stu-id="a9f5b-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="a9f5b-107">Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="a9f5b-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>