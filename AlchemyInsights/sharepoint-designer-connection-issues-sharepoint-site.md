---
title: Anslutningsproblem med SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511562"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="10617-102">Anslutningsproblem med SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="10617-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="10617-103">Om Det finns anslutningsproblem med SharePoint Designer på SharePoint-webbplatser kan du prova följande vanliga lösningar.</span><span class="sxs-lookup"><span data-stu-id="10617-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="10617-104">Steg 1: Kontrollera att SharePoint Designer 2013 har uppdaterats med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) och [den 2 augusti 2016-uppdateringen för SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="10617-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="10617-105">Steg 2: Rensa de lokala cachefilerna:</span><span class="sxs-lookup"><span data-stu-id="10617-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="10617-106">Stäng SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="10617-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="10617-107">På den lokala datorn tar du bort alla filer som finns i var och en av följande mappar.</span><span class="sxs-lookup"><span data-stu-id="10617-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="10617-108">%APPDATA%\Microsoft\Webbservertillägg\Cache</span><span class="sxs-lookup"><span data-stu-id="10617-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="10617-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="10617-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="10617-110">%USERPROFILE%\AppData\Lokal\Microsoft\WebbplatsCache</span><span class="sxs-lookup"><span data-stu-id="10617-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="10617-111">Öppna SharePoint Designer 2013 och ange kontot igen för att se om det fungerar.</span><span class="sxs-lookup"><span data-stu-id="10617-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="10617-112">Steg 3: [Aktivera modern autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="10617-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="10617-113">Steg 4: Administratörer måste **tillåta anpassade skript** i SharePoint Admin Center-inställningarna för att tillåta SharePoint Designer-anslutningen.</span><span class="sxs-lookup"><span data-stu-id="10617-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="10617-114">Mer information finns i [Tillåt eller förhindra anpassat skript.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="10617-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


