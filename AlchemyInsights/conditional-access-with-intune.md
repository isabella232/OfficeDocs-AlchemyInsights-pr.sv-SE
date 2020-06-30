---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931454"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="31fea-102">Villkorlig åtkomst med Intune</span><span class="sxs-lookup"><span data-stu-id="31fea-102">Conditional Access with Intune</span></span>

<span data-ttu-id="31fea-103">Om du använder **villkorlig åtkomst** med Intune krävs 3 steg:</span><span class="sxs-lookup"><span data-stu-id="31fea-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="31fea-104">Skapa en **efterlevnadsprincip** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="31fea-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="31fea-105">En enhet måste till exempel ha en stift på minst 6 siffror innan den anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="31fea-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="31fea-106">Skapa en **princip för villkorlig åtkomst** som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser.</span><span class="sxs-lookup"><span data-stu-id="31fea-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="31fea-107">[En](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) enhet måste till exempel vara kompatibel innan den får åtkomst till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="31fea-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="31fea-108">Se till att både **efterlevnadsprinciper** och **principer för villkorlig åtkomst** är inriktade på önskade grupper av användare.</span><span class="sxs-lookup"><span data-stu-id="31fea-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="31fea-109">Detta kan kräva att du skapar specifika grupper av användare i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31fea-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="31fea-110">**Användbara länkar:**</span><span class="sxs-lookup"><span data-stu-id="31fea-110">**Helpful links:**</span></span>

[<span data-ttu-id="31fea-111">Översikt över enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="31fea-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="31fea-112">Felsöka certifikatutfärdar</span><span class="sxs-lookup"><span data-stu-id="31fea-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="31fea-113">Felsökningsprincip</span><span class="sxs-lookup"><span data-stu-id="31fea-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="31fea-114">För att skydda e-post (Exchange online) från åtkomst av icke-kompatibla enheter måste båda dokumenten följas:</span><span class="sxs-lookup"><span data-stu-id="31fea-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="31fea-115">Skydda e-poståtkomst från enheter som använder EAS</span><span class="sxs-lookup"><span data-stu-id="31fea-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="31fea-116">Skydda e-poståtkomst från enheter med moderna autentiseringsklienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="31fea-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)