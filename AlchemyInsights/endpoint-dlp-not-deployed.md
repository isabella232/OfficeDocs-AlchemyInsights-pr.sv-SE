---
title: Slutpunkt DLP har inte distribuerats till användarens enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731869"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="f6e0c-102">Slutpunkt DLP har inte distribuerats till användarens enhet</span><span class="sxs-lookup"><span data-stu-id="f6e0c-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="f6e0c-103">Om DLP-inställningen (Endpoint data loss prevention) inte har tillämpats på en användares enhet bekräftar du att du uppfyller följande krav:</span><span class="sxs-lookup"><span data-stu-id="f6e0c-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="f6e0c-104">Windows 10 x64 version 1809 eller senare installeras på enheten.</span><span class="sxs-lookup"><span data-stu-id="f6e0c-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="f6e0c-105">Klientversion mot skadlig programvara version 4.18.2009.7 eller senare installeras.</span><span class="sxs-lookup"><span data-stu-id="f6e0c-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="f6e0c-106">Enheten är **något av** följande:</span><span class="sxs-lookup"><span data-stu-id="f6e0c-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="f6e0c-107">Azure Active Directory (AAD)-ansluten</span><span class="sxs-lookup"><span data-stu-id="f6e0c-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="f6e0c-108">Hybrid Azure AD-ansluten</span><span class="sxs-lookup"><span data-stu-id="f6e0c-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="f6e0c-109">AAD-registrerad</span><span class="sxs-lookup"><span data-stu-id="f6e0c-109">AAD registered</span></span>

- <span data-ttu-id="f6e0c-110">För att tillämpa principåtgärder ser du till att Microsoft Chromium Edge-webbläsaren är installerad på slutpunktsenheten.</span><span class="sxs-lookup"><span data-stu-id="f6e0c-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="f6e0c-111">Ytterligare krav för distribution av slutpunkt DLP finns i Komma [igång med dataförlustskydd i slutpunkten.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="f6e0c-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>