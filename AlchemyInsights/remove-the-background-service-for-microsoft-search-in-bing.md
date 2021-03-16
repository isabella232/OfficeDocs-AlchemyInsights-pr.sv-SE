---
title: Ta bort bakgrundstjänsten för Microsoft Search i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816339"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="56666-102">Ta bort bakgrundstjänsten för Microsoft Search i Bing</span><span class="sxs-lookup"><span data-stu-id="56666-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="56666-103">Om du vill ta bort bakgrundstjänsten för Microsoft Search i Bing kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="56666-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="56666-104">Så här återgår du till de ursprungliga inställningarna för sökmotor:</span><span class="sxs-lookup"><span data-stu-id="56666-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="56666-105">a.</span><span class="sxs-lookup"><span data-stu-id="56666-105">a.</span></span> <span data-ttu-id="56666-106">Inaktivera **Använd Bing som [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) standardsökmotor.**</span><span class="sxs-lookup"><span data-stu-id="56666-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="56666-107">b.</span><span class="sxs-lookup"><span data-stu-id="56666-107">b.</span></span> <span data-ttu-id="56666-108">[Gå till administrationscentret för Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) och avmarkera inställningen som påverkar alla användare i organisationen.</span><span class="sxs-lookup"><span data-stu-id="56666-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="56666-109">Så här tar du bort bakgrundstjänsten från en enskild enhet:</span><span class="sxs-lookup"><span data-stu-id="56666-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="56666-110">a.</span><span class="sxs-lookup"><span data-stu-id="56666-110">a.</span></span> <span data-ttu-id="56666-111">Välj **Kontrollpanelen i > Program > Program och funktioner**.</span><span class="sxs-lookup"><span data-stu-id="56666-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="56666-112">b.</span><span class="sxs-lookup"><span data-stu-id="56666-112">b.</span></span> <span data-ttu-id="56666-113">Högerklicka på **Microsoft Search i Bing** under listan över installerade program och klicka sedan på **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="56666-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="56666-114">Om du vill ta bort bakgrundstjänsten från flera enheter i organisationen loggar du in som administratör och kör följande kommando i ett skript:</span><span class="sxs-lookup"><span data-stu-id="56666-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
