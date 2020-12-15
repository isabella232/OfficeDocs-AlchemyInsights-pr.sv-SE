---
title: Logga in på Microsoft Edge manuellt
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678848"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="58c89-102">Logga in på Microsoft Edge manuellt</span><span class="sxs-lookup"><span data-stu-id="58c89-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="58c89-103">Om en användare inte loggas in automatiskt under en första körnings upplevelse kan användaren logga in manuellt via webbläsarens inställningar eller den utfällbara profilen.</span><span class="sxs-lookup"><span data-stu-id="58c89-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="58c89-104">Hantera inloggning genom att använda följande principer:</span><span class="sxs-lookup"><span data-stu-id="58c89-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="58c89-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – för att säkerställa att en användare alltid har en arbets profil i Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="58c89-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="58c89-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -för att begränsa inloggning till en uppsättning betrodda konton.</span><span class="sxs-lookup"><span data-stu-id="58c89-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="58c89-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – om du vill inaktivera inloggning eller tvinga användare att logga in.</span><span class="sxs-lookup"><span data-stu-id="58c89-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

