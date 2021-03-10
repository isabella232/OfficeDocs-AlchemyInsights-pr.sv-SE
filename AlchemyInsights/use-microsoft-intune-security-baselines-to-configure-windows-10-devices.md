---
title: Använda säkerhetsbaslinjer för Microsoft Intune för att konfigurera Windows 10-enheter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696383"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="89c86-102">Använd säkerhetsbaslinjerna för Microsoft Intune för att konfigurera Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="89c86-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="89c86-103">Intune-säkerhetsbaslinjer hjälper till att skydda användare och enheter.</span><span class="sxs-lookup"><span data-stu-id="89c86-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="89c86-104">Säkerhetsbaslinjer är Windows-inställningarnas förkonfigurerade grupper som används för att använda en känd grupp med inställningar och standardvärden som rekommenderas av relevanta säkerhetsteam.</span><span class="sxs-lookup"><span data-stu-id="89c86-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="89c86-105">Genom att skapa en säkerhetsbaslinjeprofil i Intune skapar du en mall som består av flera konfigurationsprofiler för enheter.</span><span class="sxs-lookup"><span data-stu-id="89c86-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="89c86-106">När du distribuerar säkerhetsbaslinjer till grupper av användare eller enheter tillämpas inställningarna på enheter som körs på Windows 10 eller senare versioner.</span><span class="sxs-lookup"><span data-stu-id="89c86-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="89c86-107">Till exempel aktiverar Microsofts baslinje för hantering av mobila enheter (MDM) automatiskt (1) BitLocker för flyttbara enheter, (2) kräver lösenordet för att låsa upp en enhet och (3) inaktiverar grundläggande autentisering.</span><span class="sxs-lookup"><span data-stu-id="89c86-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="89c86-108">När ett standardvärde inte fungerar för din miljö kan du anpassa baslinjen så att de inställningar du behöver används.</span><span class="sxs-lookup"><span data-stu-id="89c86-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="89c86-109">Säkerhetsbaslinjer hjälper också till att upprätta ett säkert arbetsflöde i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="89c86-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="89c86-110">Följande är några av fördelarna med den här funktionen:</span><span class="sxs-lookup"><span data-stu-id="89c86-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="89c86-111">En säkerhetsbaslinje innehåller metodtips och rekommendationer för inställningar som påverkar säkerheten.</span><span class="sxs-lookup"><span data-stu-id="89c86-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="89c86-112">Eftersom Intune samarbetar med Windows-säkerhetsteamet som skapar baslinjer för grupprinciper, baseras de här rekommendationerna på stabil vägledning och omfattande erfarenhet.</span><span class="sxs-lookup"><span data-stu-id="89c86-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="89c86-113">Om du är nybörjare i Intune och är osäker på var du ska börja kommer säkerhetsbaslinjer att hjälpa dig att snabbt skapa och distribuera en säker profil.</span><span class="sxs-lookup"><span data-stu-id="89c86-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="89c86-114">Om du använder en grupprincip är det mycket enklare att migrera till Intune för hanteringsändamål med säkerhetsbaslinjer, eftersom dessa säkerhetsbaslinjer är inbyggda i Intune och innehåller avancerade funktioner för hantering.</span><span class="sxs-lookup"><span data-stu-id="89c86-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="89c86-115">Mer information finns i Windows [säkerhetsbaslinjer och](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) hantering [av mobila enheter.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="89c86-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>