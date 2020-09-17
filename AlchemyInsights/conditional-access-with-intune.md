---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807677"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="59b64-102">Villkorlig åtkomst med Intune</span><span class="sxs-lookup"><span data-stu-id="59b64-102">Conditional Access with Intune</span></span>

<span data-ttu-id="59b64-103">Användning av  **villkorsstyrd åtkomst**  med Intune kräver tre steg:</span><span class="sxs-lookup"><span data-stu-id="59b64-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="59b64-104">Skapa en  **efterlevnadsprincip**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) för att definiera inställningar som måste uppfyllas innan enheten anses uppfylla kraven.</span><span class="sxs-lookup"><span data-stu-id="59b64-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="59b64-105">En enhet måste till exempel ha en PIN-kod på minst 6 siffror innan den anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="59b64-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="59b64-106">Skapa en **princip för villkorsstyrd åtkomst**  som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att få åtkomst till resurserna.</span><span class="sxs-lookup"><span data-stu-id="59b64-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="59b64-107">En enhet måste [till exempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) vara kompatibel innan du kan komma åt företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="59b64-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="59b64-108">Se till att båda reglerna för **efterlevnad**  och  **villkorsstyrd åtkomst**  är riktade till önskade grupper av användare.</span><span class="sxs-lookup"><span data-stu-id="59b64-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="59b64-109">Detta kan kräva att specifika användar grupper skapas i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59b64-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="59b64-110">**Användbara länkar:**</span><span class="sxs-lookup"><span data-stu-id="59b64-110">**Helpful links:**</span></span>

[<span data-ttu-id="59b64-111">Översikt över enhetens efterlevnad</span><span class="sxs-lookup"><span data-stu-id="59b64-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="59b64-112">Felsöka CA</span><span class="sxs-lookup"><span data-stu-id="59b64-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="59b64-113">Fel söknings princip</span><span class="sxs-lookup"><span data-stu-id="59b64-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="59b64-114">För att skydda e-post (Exchange Online) från åtkomst via icke-kompatibla enheter måste båda dokumenten följas:</span><span class="sxs-lookup"><span data-stu-id="59b64-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="59b64-115">Skydda e-poståtkomst från enheter med hjälp av EAS</span><span class="sxs-lookup"><span data-stu-id="59b64-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="59b64-116">Skydda e-poståtkomst från enheter med moderna klienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="59b64-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)