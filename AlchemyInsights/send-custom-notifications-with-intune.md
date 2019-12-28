---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886875"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="aace6-102">Så här skickar du anpassade meddelanden till användare av hanterade iOS-och Android-enheter</span><span class="sxs-lookup"><span data-stu-id="aace6-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="aace6-103">Anpassade meddelanden för Intune bearbetas av företagsportalappen på en användares enhet.</span><span class="sxs-lookup"><span data-stu-id="aace6-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="aace6-104">Appen skapar sedan push-meddelande på den enheten.</span><span class="sxs-lookup"><span data-stu-id="aace6-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="aace6-105">Följande är enhets förutsättningar för att stödja mottagandet av anpassade meddelanden och för att appen ska skapa push-meddelandet:</span><span class="sxs-lookup"><span data-stu-id="aace6-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="aace6-106">Enheten måste ha företagsportalappen installerad.</span><span class="sxs-lookup"><span data-stu-id="aace6-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="aace6-107">Enheten måste tillåta företagsportalappen att skicka push-meddelanden.</span><span class="sxs-lookup"><span data-stu-id="aace6-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="aace6-108">När appen installeras eller uppdateras uppmanas användaren att tillåta meddelanden.</span><span class="sxs-lookup"><span data-stu-id="aace6-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="aace6-109">Android-enheter måste ha Google Play-tjänster installerade.</span><span class="sxs-lookup"><span data-stu-id="aace6-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="aace6-110">Enheten måste vara registrerad med Intune.</span><span class="sxs-lookup"><span data-stu-id="aace6-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="aace6-111">Mer information, inklusive hur du skickar ett meddelande, finns i [funktions dokumentationen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="aace6-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
