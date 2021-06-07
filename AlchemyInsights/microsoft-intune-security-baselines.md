---
title: Använda Microsoft Intune säkerhetsbaslinjer för att konfigurera Windows 10 enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794129"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="7eb9f-102">Använda Microsoft Intune säkerhetsbaslinjer för att konfigurera Windows 10 enheter</span><span class="sxs-lookup"><span data-stu-id="7eb9f-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="7eb9f-103">Intune-säkerhetsbaslinjer hjälper till att skydda användare och enheter.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="7eb9f-104">Säkerhetsbaslinjer är Windows förkonfigurerade grupper som används för att tillämpa en känd grupp med inställningar och standardvärden som rekommenderas av relevanta säkerhetsteam.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="7eb9f-105">Genom att skapa en profil för säkerhetsbaslinje i Intune skapar du en mall som består av flera enhetskonfigurationsprofiler.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="7eb9f-106">När du distribuerar säkerhetsbaslinjer till grupper av användare eller enheter tillämpas inställningarna på enheter som körs på Windows 10 eller senare.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="7eb9f-107">Microsofts baslinje för hantering av mobila enheter (MDM) aktiverar till exempel automatiskt BitLocker för flyttbara enheter, kräver lösenordet för att låsa upp en enhet och inaktiverar grundläggande autentisering.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="7eb9f-108">När ett standardvärde inte fungerar för din miljö kan du anpassa originalplanen så att de inställningar du behöver används.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="7eb9f-109">Säkerhetsbaslinjer hjälper också till att upprätta ett säkert arbetsflöde av helt slut i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="7eb9f-110">En säkerhetsbaslinje innehåller metodtips och rekommendationer för inställningar som påverkar säkerheten.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="7eb9f-111">Intune-partner med Windows säkerhetsteam som skapar baslinjer för gruppprinciper, så dessa rekommendationer baseras på stabil vägledning och omfattande erfarenhet.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="7eb9f-112">Om du är nybörjare i Intune och är osäker på var du ska börja kan du med hjälp av säkerhetsbaslinjer snabbt skapa och distribuera en säker profil.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="7eb9f-113">Om du använder en grupprincip är det mycket enklare att migrera till Intune för hanteringsändamål med säkerhetsbaslinjer eftersom de är inbyggda i Intune och innehåller avancerade hanteringsfunktioner.</span><span class="sxs-lookup"><span data-stu-id="7eb9f-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="7eb9f-114">Mer information finns i [Windows baslinjer för säkerhet](/windows/security/threat-protection/windows-security-baselines) och hantering av mobila [enheter.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="7eb9f-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

