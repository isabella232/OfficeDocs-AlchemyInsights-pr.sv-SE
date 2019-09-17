---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992330"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="6bda3-102">Så här skickar du anpassade meddelanden till användare av hanterade iOS-och Android-enheter</span><span class="sxs-lookup"><span data-stu-id="6bda3-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="6bda3-103">Anpassade meddelanden för Intune bearbetas av företagsportalappen på en användares enhet.</span><span class="sxs-lookup"><span data-stu-id="6bda3-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="6bda3-104">Appen skapar sedan push-meddelande på den enheten.</span><span class="sxs-lookup"><span data-stu-id="6bda3-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="6bda3-105">Följande är enhets förutsättningar för att stödja mottagandet av anpassade meddelanden och för att appen ska skapa push-meddelandet:</span><span class="sxs-lookup"><span data-stu-id="6bda3-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="6bda3-106">Enheten måste ha företagsportalappen installerad.</span><span class="sxs-lookup"><span data-stu-id="6bda3-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="6bda3-107">Enheten måste tillåta företagsportalappen att skicka push-meddelanden.</span><span class="sxs-lookup"><span data-stu-id="6bda3-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="6bda3-108">När appen installeras eller uppdateras uppmanas användaren att tillåta meddelanden.</span><span class="sxs-lookup"><span data-stu-id="6bda3-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="6bda3-109">Android-enheter måste ha Google Play-tjänster installerade.</span><span class="sxs-lookup"><span data-stu-id="6bda3-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="6bda3-110">Enheten måste vara registrerad med Intune.</span><span class="sxs-lookup"><span data-stu-id="6bda3-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="6bda3-111">Mer information, inklusive hur du skickar ett meddelande, finns i [funktions dokumentationen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="6bda3-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
