---
title: Microsoft Edge-support för Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584009"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="c865a-102">Microsoft Edge-support för Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="c865a-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="c865a-103">Application Guard är utformat för Windows 10 och Microsoft Edge och använder ett maskin varu isolerings sätt som låter en användare navigera från en icke betrodd webbplats i en isolerad, Hyper-V-aktiverad behållare, avgränsas från operativ systemet.</span><span class="sxs-lookup"><span data-stu-id="c865a-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="c865a-104">En företags administratör definierar en lista över tillförlitliga webbplatser, moln resurser och interna nätverk.</span><span class="sxs-lookup"><span data-stu-id="c865a-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="c865a-105">När en användare besöker en webbplats som inte finns med i listan öppnar Microsoft Edge webbplatsen i behållaren.</span><span class="sxs-lookup"><span data-stu-id="c865a-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="c865a-106">Det innebär att om webbplatsen blir skadlig kan värddatorn vara skyddad och angripare kommer inte till företags data.</span><span class="sxs-lookup"><span data-stu-id="c865a-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="c865a-107">Installation av tillägg i behållaren stöds enligt Microsoft Edge version 81 och kan styras via en princip.</span><span class="sxs-lookup"><span data-stu-id="c865a-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="c865a-108">Den updateURL-adress som används i ExtensionInstallForcelist-principen ska läggas till som en neutral resurs i principerna för nätverks isolering som används av Application Guard.</span><span class="sxs-lookup"><span data-stu-id="c865a-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="c865a-109">Mer information finns i [Microsoft Edge support för Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="c865a-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
