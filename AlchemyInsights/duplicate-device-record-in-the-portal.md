---
title: Dubblerad enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790175"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="434b1-102">Dubblerad enhetspost i portalen</span><span class="sxs-lookup"><span data-stu-id="434b1-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="434b1-103">Du kan se två poster för en enhet i portalen om enheten inte korrekt rapporterar status för samhantering till Configuration Manager-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="434b1-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="434b1-104">För att kontrollera statusen för samhantering av en enhet tittar du i kolumnen **Samhanterad** för enheten i Configuration Manager-konsolen.</span><span class="sxs-lookup"><span data-stu-id="434b1-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="434b1-105">Om kolumnen inte visas kan du lägga till den genom att högerklicka på en kolumnrubrik och välja den i listan.</span><span class="sxs-lookup"><span data-stu-id="434b1-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="434b1-106">Värdet på Samhanterad ska vara **Ja**.</span><span class="sxs-lookup"><span data-stu-id="434b1-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="434b1-107">Om värdet är **Nej** öppnar du Configuration Manager-klientappleten på klientenheten och markerar egenskapen **Samhantering** på fliken Allmänt.</span><span class="sxs-lookup"><span data-stu-id="434b1-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="434b1-108">Om värdet är **Aktiverat** antyder det problem med klientkommunikationen med hanteringsplatsen.</span><span class="sxs-lookup"><span data-stu-id="434b1-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="434b1-109">Läs **CcmMessaging.log** på enheten för att undersöka potentiella anslutningsproblem.</span><span class="sxs-lookup"><span data-stu-id="434b1-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="434b1-110">Om värdet är **Inaktiverat** och enheten är registrerad i Intune ska du kontrollera att enheten har tagit emot principen för samhantering genom att läsa **CoManagementHandler.log** på enheten.</span><span class="sxs-lookup"><span data-stu-id="434b1-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
