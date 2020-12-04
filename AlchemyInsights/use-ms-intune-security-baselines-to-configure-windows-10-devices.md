---
title: Använda säkerhets bas linjer i Microsoft Intune för att konfigurera Windows 10-enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573787"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="0ce2f-102">Använda säkerhets bas linjer i Microsoft Intune för att konfigurera Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="0ce2f-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="0ce2f-103">Intune säkerhets bas linjer hjälper dig att skydda användare och enheter.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0ce2f-104">Säkerhets bas linjer är Windows-inställningar ' förkonfigurerade grupper som används för att tillämpa en känd uppsättning inställningar och standardvärden som rekommenderas av relevanta säkerhets team.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0ce2f-105">Genom att skapa en säkerhets bas profil i Intune skapar du en mall som består av flera enheter-konfigurations profiler.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0ce2f-106">När du distribuerar säkerhets bas linjer till grupper med användare eller enheter tillämpas inställningarna på enheter som körs på Windows 10 eller senare.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="0ce2f-107">Till exempel kan MDM-säkerhetsfunktionen (1) Aktivera BitLocker för flyttbara enheter (2) kräva lösen ordet för att låsa upp en enhet och (3) inaktiverar grundläggande verifikation.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="0ce2f-108">När ett standardvärde inte fungerar för din miljö kan du anpassa bas linjen för att tillämpa de inställningar du behöver.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0ce2f-109">Säkerhets bas linjer hjälper dig också att etablera ett säkert arbets flöde från ett slutdatum till en slutpunkt i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0ce2f-110">Här är några av fördelarna med följande:</span><span class="sxs-lookup"><span data-stu-id="0ce2f-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="0ce2f-111">En säkerhets plan innehåller de bästa metoderna och rekommendationerna för inställningar som påverkar säkerheten.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0ce2f-112">Eftersom Intune-partners med Windows säkerhets team som skapar bas linjer för grup principer baseras dessa rekommendationer på heltäckande vägledning och omfattande upplevelse.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="0ce2f-113">Om du är nybörjare på Intune och är osäker på var du ska starta, kan du med hjälp av säkerhets rikt linjer snabbt skapa och distribuera en säker profil.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="0ce2f-114">Om du för närvarande använder en grup princip är det mycket enklare att migrera till Intune för hantering med säkerhets bas linjer, eftersom de är inbyggda i Intune och innehåller funktioner för överkanten för hantering.</span><span class="sxs-lookup"><span data-stu-id="0ce2f-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="0ce2f-115">Mer information finns i [säkerhets bas linjer för Windows](https://go.microsoft.com/fwlink/?linkid=2141503) och [hantering av mobila enheter](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="0ce2f-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>