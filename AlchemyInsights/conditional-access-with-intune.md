---
title: Villkorsstyrd åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704804"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="75fb5-102">Villkorsstyrd åtkomst med Intune</span><span class="sxs-lookup"><span data-stu-id="75fb5-102">Conditional Access with Intune</span></span>

<span data-ttu-id="75fb5-103">För  **användning av villkorsstyrd**  åtkomst med Intune krävs tre steg:</span><span class="sxs-lookup"><span data-stu-id="75fb5-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="75fb5-104">Skapa en  **efterlevnadsprincip** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="75fb5-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="75fb5-105">En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="75fb5-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="75fb5-106">Skapa en **princip för villkorsstyrd**  åtkomst som definierar vilka resurser som ska skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser.</span><span class="sxs-lookup"><span data-stu-id="75fb5-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="75fb5-107">[En enhet måste till](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  exempel vara kompatibel innan åtkomst ges till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="75fb5-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="75fb5-108">Se till **att både efterlevnadsprinciper**  **och villkorsstyrda**  åtkomstprinciper är riktade till önskade grupper av användare.</span><span class="sxs-lookup"><span data-stu-id="75fb5-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="75fb5-109">Det kan kräva att du skapar särskilda grupper av användare i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="75fb5-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="75fb5-110">**Användbara länkar:**</span><span class="sxs-lookup"><span data-stu-id="75fb5-110">**Helpful links:**</span></span>

[<span data-ttu-id="75fb5-111">Översikt över enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="75fb5-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="75fb5-112">Felsökning av certifikatutfärdare</span><span class="sxs-lookup"><span data-stu-id="75fb5-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="75fb5-113">Felsökningsprincip</span><span class="sxs-lookup"><span data-stu-id="75fb5-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="75fb5-114">För att skydda e-post (Exchange online) från åtkomst från enheter som inte är kompatibla måste båda dokumenten följas:</span><span class="sxs-lookup"><span data-stu-id="75fb5-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="75fb5-115">Skydda e-poståtkomst från enheter med EAS</span><span class="sxs-lookup"><span data-stu-id="75fb5-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="75fb5-116">Skydda e-poståtkomst från enheter som använder moderna autentiseringsklienter som Outlook</span><span class="sxs-lookup"><span data-stu-id="75fb5-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)