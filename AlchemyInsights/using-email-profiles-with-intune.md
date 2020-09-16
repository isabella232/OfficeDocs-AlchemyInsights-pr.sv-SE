---
title: Använda e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653306"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="6a2a7-102">Använda e-postprofiler med Intune</span><span class="sxs-lookup"><span data-stu-id="6a2a7-102">Using email profiles with Intune</span></span>

<span data-ttu-id="6a2a7-103">Intune kan användas för att skapa och distribuera e-postprofiler för den inbyggda (inbyggda) e-postklienten på flera plattformar.</span><span class="sxs-lookup"><span data-stu-id="6a2a7-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="6a2a7-104">Information om några av de begränsningar som gäller för e-profiler, inklusive hur befintliga profiler hanteras och hur du tar bort e-profilerna, finns i avsnittet [lägga till inställningar för e-post på enheter med Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="6a2a7-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="6a2a7-105">Mer information om hur du skapar e-postprofiler för varje enhets plattform finns i:</span><span class="sxs-lookup"><span data-stu-id="6a2a7-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="6a2a7-106">Android-enhetens inställningar för att konfigurera e-post, auktorisering och synkronisering i Intune</span><span class="sxs-lookup"><span data-stu-id="6a2a7-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="6a2a7-107">Lägga till e-postinställningar för iOS-och iPad-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6a2a7-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="6a2a7-108">Inställningar för e-postprofil i Microsoft Intune för enheter med Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="6a2a7-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="6a2a7-109">Inställningar för e-postprofil för enheter med Windows 10 i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6a2a7-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="6a2a7-110">**Vanligt problem med synkronisering**</span><span class="sxs-lookup"><span data-stu-id="6a2a7-110">**Common syncing issue**</span></span>

<span data-ttu-id="6a2a7-111">**En KNOX on Android-e-postprofil hindrar att användarnas kontakter, kalender och uppgifter synkroniseras till användar enheter.**</span><span class="sxs-lookup"><span data-stu-id="6a2a7-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="6a2a7-112">I e-postprofilen KNOX på Android KNOX kan administratören välja att avgöra vilka innehålls typer som synkroniseras till enheten genom att ställa in dem på aktive rad.</span><span class="sxs-lookup"><span data-stu-id="6a2a7-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="6a2a7-113">Om inställningen för någon av innehålls typerna är inställd på **ej konfigurerad** (standard) synkroniseras inte den innehålls typen automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6a2a7-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="6a2a7-114">En användare kan aktivera den innehålls typ de vill ha direkt på enheten, men denna konfiguration skrivs över av Intune-inställningarna och synkroniseringen stoppas för innehålls typen.</span><span class="sxs-lookup"><span data-stu-id="6a2a7-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

