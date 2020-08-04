---
title: Använda e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555760"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="f1005-102">Använda e-postprofiler med Intune</span><span class="sxs-lookup"><span data-stu-id="f1005-102">Using email profiles with Intune</span></span>

<span data-ttu-id="f1005-103">Intune kan användas för att skapa och distribuera e-postprofiler för den inbyggda (inbyggda) e-postklienten på flera enhetsplattformar.</span><span class="sxs-lookup"><span data-stu-id="f1005-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="f1005-104">Information om några av de begränsningar som är kopplade till e-postprofiler, inklusive hur förekomsten av befintliga profiler hanteras och hur du tar bort e-postprofiler, finns [i Lägga till e-postinställningar på enheter som använder Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="f1005-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="f1005-105">Mer information om hur du skapar e-postprofiler för varje enhetsplattform finns i:</span><span class="sxs-lookup"><span data-stu-id="f1005-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="f1005-106">Inställningar för Android-enheter för att konfigurera e-post, autentisering och synkronisering i Intune</span><span class="sxs-lookup"><span data-stu-id="f1005-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="f1005-107">Lägga till e-postinställningar för iOS- och iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f1005-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="f1005-108">Inställningar för e-postprofiler i Microsoft Intune för enheter som kör Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="f1005-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="f1005-109">Inställningar för e-postprofiler för enheter som kör Windows 10 i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f1005-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="f1005-110">**Vanligt synkroniseringsproblem**</span><span class="sxs-lookup"><span data-stu-id="f1005-110">**Common syncing issue**</span></span>

<span data-ttu-id="f1005-111">**En KNOX på Android-e-postprofil förhindrar att användarna kontakter, kalender och uppgifter synkroniseras med användarenheter.**</span><span class="sxs-lookup"><span data-stu-id="f1005-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="f1005-112">Knox på Android KNOX-e-postprofilen ger administratören möjlighet att bestämma vilka innehållstyper som ska synkroniseras med enheten genom att ställa in var och en på aktiverad.</span><span class="sxs-lookup"><span data-stu-id="f1005-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="f1005-113">Om inställningen för någon av innehållstyperna är inställd **på Inte konfigurerad** (standard) synkroniseras inte innehållstypen automatiskt.</span><span class="sxs-lookup"><span data-stu-id="f1005-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="f1005-114">En användare kan aktivera den innehållstyp de vill ha direkt på enheten manuellt, men den konfigurationen skrivs över av principinställningen Intune och synkroniseringen stoppas för den innehållstypen.</span><span class="sxs-lookup"><span data-stu-id="f1005-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

