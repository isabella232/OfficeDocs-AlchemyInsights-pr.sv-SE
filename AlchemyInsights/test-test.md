---
title: Villkor som saknas i SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766871"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="60cbc-102">Aktivera Bitlocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="60cbc-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="60cbc-103">Intune Endpoint Protection Policy kan användas för att konfigurera Boitlocker-krypteringsinställningar för Windows-enheter enligt beskrivningen i : Windows10-inställningar (och senare) för att skydda enheter som använder Intune</span><span class="sxs-lookup"><span data-stu-id="60cbc-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="60cbc-104">Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk bitlockerkryptering som utlöses utan tillämpning av MDM-principen.</span><span class="sxs-lookup"><span data-stu-id="60cbc-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="60cbc-105">Detta kan påverka tillämpningen av principen om icke-standardinställningarna är konfigurerade.</span><span class="sxs-lookup"><span data-stu-id="60cbc-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="60cbc-106">Se Vanliga frågor och svar för mer information.</span><span class="sxs-lookup"><span data-stu-id="60cbc-106">See FAQ for more detail.</span></span>


<span data-ttu-id="60cbc-107">Vanliga  frågor och svar F: Vilka versioner av Windows stöder enhetskryptering med hjälp av slutpunktsskyddsprincipen?</span><span class="sxs-lookup"><span data-stu-id="60cbc-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="60cbc-108"> S: Inställningarna i Intune Endpoint Protection Policy implementeras med Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="60cbc-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="60cbc-109">Inte alla utgåvor eller versioner av Windows stöder Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="60cbc-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="60cbc-110">Vid denna tid Windows Editions: Enterprise; Utbildning, mobil, mobilt företag och professional (från bygg 1809 och framåt) stöds.</span><span class="sxs-lookup"><span data-stu-id="60cbc-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="60cbc-111">F: Om en enhet redan är krypterad med Bitlocker med hjälp av OS-standardinställningarna för krypteringsmetod och chifferstyrka (XTS-AES-128) kommer att tillämpa en princip med olika inställningar automatiskt utlösa omkryptering av enheten med de nya inställningarna?</span><span class="sxs-lookup"><span data-stu-id="60cbc-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="60cbc-112">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="60cbc-112">A: No.</span></span> <span data-ttu-id="60cbc-113">För att kunna tillämpa de nya chifferinställningarna måste enheten först dekrypteras.</span><span class="sxs-lookup"><span data-stu-id="60cbc-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="60cbc-114">För enheter som registreras med Autopilot utlöses inte den automatiska kryptering som skulle ske under OOBE förrän Intune-principen utvärderas, vilket gör att de principbaserade inställningarna kan användas i stället för OS-standardinställningarna</span><span class="sxs-lookup"><span data-stu-id="60cbc-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="60cbc-115">F Om en enhet krypteras som ett resultat av tillämpningen av Intune-principen kommer den att dekrypteras när den principen tas bort?</span><span class="sxs-lookup"><span data-stu-id="60cbc-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="60cbc-116">S: Borttagning av krypteringsrelaterad princip resulterar INTE i dekryptering av de enheter som har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="60cbc-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="60cbc-117">F: Varför visar intune Compliance-principen att min enhet inte har "Bitlocker Enabled" men det är?</span><span class="sxs-lookup"><span data-stu-id="60cbc-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="60cbc-118">S: Inställningen "Bitlocker enabled" i intune-efterlevnadsprincipen använder DHA-klienten (Windows Device Health Attestation).</span><span class="sxs-lookup"><span data-stu-id="60cbc-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="60cbc-119">Den här klienten mäter endast enhetstillstånd vid uppstart.</span><span class="sxs-lookup"><span data-stu-id="60cbc-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="60cbc-120">Så om en enhet inte har startats om sedan bitlocker kryptering slutfördes DHA klienttjänsten kommer inte att rapportera bitlocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="60cbc-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>