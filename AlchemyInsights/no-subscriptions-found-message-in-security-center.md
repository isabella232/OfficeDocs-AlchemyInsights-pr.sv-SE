---
title: Inga prenumerationer hittades i Säkerhetscenter
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714389"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="d6013-102">Inga prenumerationer hittades i Säkerhetscenter</span><span class="sxs-lookup"><span data-stu-id="d6013-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="d6013-103">Om du får meddelandet "Inga prenumerationer hittades" när du öppnar Microsoft Defender Säkerhetscenter innebär det att Azure Active Directory (AAD) som används för att logga in användaren på portalen inte har någon Microsoft Defender ATP-licens.</span><span class="sxs-lookup"><span data-stu-id="d6013-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="d6013-104">Licenserna för Windows E5 och Office E5 är separata licenser.</span><span class="sxs-lookup"><span data-stu-id="d6013-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="d6013-105">Öppna ett supportärende om licensen har köpts men inte etablerats i den här AAD-instansen.</span><span class="sxs-lookup"><span data-stu-id="d6013-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="d6013-106">Antingen har du:</span><span class="sxs-lookup"><span data-stu-id="d6013-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="d6013-107">Ett möjligt problem med licensetablering.</span><span class="sxs-lookup"><span data-stu-id="d6013-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="d6013-108">Du har oavsiktligt etablerat licensen till en annan Microsoft AAD än den som används för autentisering i tjänsten.</span><span class="sxs-lookup"><span data-stu-id="d6013-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>