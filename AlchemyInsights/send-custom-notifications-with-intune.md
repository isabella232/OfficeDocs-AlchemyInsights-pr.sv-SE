---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720664"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="92fb1-102">Skicka anpassade meddelanden till användare av hanterade iOS-och Android-enheter</span><span class="sxs-lookup"><span data-stu-id="92fb1-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="92fb1-103">Anpassade meddelanden för Intune bearbetas av företagsportalsappen på en användares enhet.</span><span class="sxs-lookup"><span data-stu-id="92fb1-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="92fb1-104">Programmet skapar sedan push-meddelandet på den enheten.</span><span class="sxs-lookup"><span data-stu-id="92fb1-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="92fb1-105">Följande är enhets förutsättningar för att stödja mottagning av anpassade meddelanden, och för appen att skapa push-meddelandet:</span><span class="sxs-lookup"><span data-stu-id="92fb1-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="92fb1-106">Programmet måste ha företagsportalsappen installerat.</span><span class="sxs-lookup"><span data-stu-id="92fb1-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="92fb1-107">Enheten måste tillåta att företagsportalsappen skickar push-meddelanden till företags portalen.</span><span class="sxs-lookup"><span data-stu-id="92fb1-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="92fb1-108">När appen installeras eller uppdateras uppmanas användaren att tillåta aviseringar.</span><span class="sxs-lookup"><span data-stu-id="92fb1-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="92fb1-109">Google Play Services måste vara installerat på Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="92fb1-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="92fb1-110">Enheten måste vara registrerad med Intune.</span><span class="sxs-lookup"><span data-stu-id="92fb1-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="92fb1-111">Mer information om hur du skickar ett meddelande finns i dokumentationen för [funktionerna](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="92fb1-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
