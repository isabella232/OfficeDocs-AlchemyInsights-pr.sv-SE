---
title: Dubblerad enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814534"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="c2b76-102">Dubblerad enhetspost i portalen</span><span class="sxs-lookup"><span data-stu-id="c2b76-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="c2b76-103">Du kan se två poster för en enhet i portalen om enheten inte korrekt rapporterar status för samhantering till Configuration Manager-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="c2b76-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="c2b76-104">För att kontrollera statusen för samhantering av en enhet tittar du i kolumnen **Samhanterad** för enheten i Configuration Manager-konsolen.</span><span class="sxs-lookup"><span data-stu-id="c2b76-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="c2b76-105">Om kolumnen inte visas kan du lägga till den genom att högerklicka på en kolumnrubrik och välja den i listan.</span><span class="sxs-lookup"><span data-stu-id="c2b76-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="c2b76-106">Värdet på Samhanterad ska vara **Ja**.</span><span class="sxs-lookup"><span data-stu-id="c2b76-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="c2b76-107">Om värdet är **Nej** öppnar du Configuration Manager-klientappleten på klientenheten och markerar egenskapen **Samhantering** på fliken Allmänt.</span><span class="sxs-lookup"><span data-stu-id="c2b76-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="c2b76-108">Om värdet är **Aktiverat** antyder det problem med klientkommunikationen med hanteringsplatsen.</span><span class="sxs-lookup"><span data-stu-id="c2b76-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="c2b76-109">Läs **CcmMessaging.log** på enheten för att undersöka potentiella anslutningsproblem.</span><span class="sxs-lookup"><span data-stu-id="c2b76-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="c2b76-110">Om värdet är **Inaktiverat** och enheten är registrerad i Intune ska du kontrollera att enheten har tagit emot principen för samhantering genom att läsa **CoManagementHandler.log** på enheten.</span><span class="sxs-lookup"><span data-stu-id="c2b76-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
