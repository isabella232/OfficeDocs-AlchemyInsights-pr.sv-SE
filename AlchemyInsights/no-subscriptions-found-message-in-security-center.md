---
title: Inga prenumerationer hittades i säkerhetscentret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544126"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="31856-102">Inga prenumerationer hittades i säkerhetscentret</span><span class="sxs-lookup"><span data-stu-id="31856-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="31856-103">Om du får meddelandet "Inga prenumerationer hittades" när du öppnar Microsoft Defender Säkerhetscenter innebär det att den Azure Active Directory (AAD) som används för att logga in användaren på portalen inte har en Microsoft Defender ATP licens.</span><span class="sxs-lookup"><span data-stu-id="31856-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="31856-104">Licenserna Windows E5 Office E5 är separata licenser.</span><span class="sxs-lookup"><span data-stu-id="31856-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="31856-105">Öppna ett supportärende om licensen har köpts men inte etablerats i den här AAD-instansen.</span><span class="sxs-lookup"><span data-stu-id="31856-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="31856-106">Du har antingen:</span><span class="sxs-lookup"><span data-stu-id="31856-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="31856-107">Ett möjligt problem med licensetablering.</span><span class="sxs-lookup"><span data-stu-id="31856-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="31856-108">Du har oavsiktligt etablerat licensen till en annan Microsoft AAD än den som används för autentisering i tjänsten.</span><span class="sxs-lookup"><span data-stu-id="31856-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>