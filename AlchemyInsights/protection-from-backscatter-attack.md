---
title: Skydd mot bakåtcatterattack
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037180"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="229c9-102">Skydd mot bakåtcatterattack</span><span class="sxs-lookup"><span data-stu-id="229c9-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="229c9-103">Bakåtcatter är rapporter om utebliven leverans (kallas även NDR-rapporter eller icke-leveranskända meddelanden) som du får för meddelanden som du inte har skickat.</span><span class="sxs-lookup"><span data-stu-id="229c9-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="229c9-104">Skräppostavs spammare förfalskar meddelandens adress **från:** och de använder ofta riktiga e-postadresser för att låna ut trovärdigheten för sina meddelanden.</span><span class="sxs-lookup"><span data-stu-id="229c9-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="229c9-105">Så om skräppostavsändare oundvikligen skickar meddelanden till mottagare som inte finns, luras nämligen mål-e-postservern i princip att skicka tillbaka det olevererbara meddelandet i en NDR till den förfalskade avsändaren i **Från:-adressen.**</span><span class="sxs-lookup"><span data-stu-id="229c9-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="229c9-106">Ytterligare information finns i [Bakåtcatter i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="229c9-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="229c9-107">**Aktivera skydd mot bakåtcatter**</span><span class="sxs-lookup"><span data-stu-id="229c9-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="229c9-108">Aktivera bakåtcatterskydd genom att följa sökvägen nedan.</span><span class="sxs-lookup"><span data-stu-id="229c9-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="229c9-109">**protection.office.com > Threat Management > Policy > Antispam > Välj policyn för skräppostfilter och redigera principen > Egenskaper för skräppost > Markera som skräppost > NDR-bakåtcatter > Ställ in den på "På"**</span><span class="sxs-lookup"><span data-stu-id="229c9-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="229c9-110">Läs följande om du tror att ett konto har komprometterats:</span><span class="sxs-lookup"><span data-stu-id="229c9-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="229c9-111">Hantera ett komprometterat e-postkonto</span><span class="sxs-lookup"><span data-stu-id="229c9-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="229c9-112">Ta bort blockerade användare från portalen begränsade användare i Office 365</span><span class="sxs-lookup"><span data-stu-id="229c9-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



