---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908727"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="a547f-102">Aktivera BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="a547f-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="a547f-103">Intune Endpoint Protection-principen kan användas för att konfigurera BitLocker-krypteringsinställningar för Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="a547f-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="a547f-104">Mer information finns i [Windows 10 (och senare) inställningar för att skydda enheter med hjälp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="a547f-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="a547f-105">Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering, som utlöses utan tillämpning av MDM-principen.</span><span class="sxs-lookup"><span data-stu-id="a547f-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="a547f-106">Detta kan påverka tillämpningen av principen om icke-standardinställningar har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="a547f-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="a547f-107">Se följande vanliga frågor och svar för mer information.</span><span class="sxs-lookup"><span data-stu-id="a547f-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="a547f-108">Information om hur du felsöker problem med BitLocker finns [i Felsöka BitLocker-principer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="a547f-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="a547f-109">**Vanliga frågor och svar**</span><span class="sxs-lookup"><span data-stu-id="a547f-109">**FAQ**</span></span>

 <span data-ttu-id="a547f-110">F: vilka utgåvor av Windows stöder enhetskryptering med hjälp av Endpoint Protection-principen?</span><span class="sxs-lookup"><span data-stu-id="a547f-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="a547f-111">A: inställningarna i Intune Endpoint Protection-principen implementeras med hjälp av [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="a547f-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="a547f-112">Inte alla utgåvor eller build-versioner av Windows stöder BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="a547f-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="a547f-113">För tillfället stöds följande Windows-utgåvor: Enterprise, Education, Mobile, Mobile Enterprise och Professional (build 1809 och senare).</span><span class="sxs-lookup"><span data-stu-id="a547f-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="a547f-114">F: om en enhet redan är krypterad med BitLocker med hjälp av OS standardinställningarna för krypteringsmetod och cipher styrka (XTS-AES-128), kommer att tillämpa en princip med olika inställningar automatiskt utlösa Omkryptering av enheten med de nya inställningarna?</span><span class="sxs-lookup"><span data-stu-id="a547f-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="a547f-115">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="a547f-115">A: No.</span></span> <span data-ttu-id="a547f-116">Om du vill använda de nya cipher-inställningarna måste enheten först dekrypteras.</span><span class="sxs-lookup"><span data-stu-id="a547f-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="a547f-117">**Anmärkning:** För enheter som registreras med autopilot utlöses inte den automatiska kryptering som skulle inträffa under OOBE förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar kan användas i stället för OPERATIVsystemets standardvärden.</span><span class="sxs-lookup"><span data-stu-id="a547f-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="a547f-118">F: om en enhet krypteras som ett resultat av tillämpningen av Intune-principen, kommer det att dekrypteras när principen tas bort?</span><span class="sxs-lookup"><span data-stu-id="a547f-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="a547f-119">S: borttagning av krypteringsrelaterade principer resulterar inte i dekryptering av enheter som har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="a547f-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="a547f-120">F: Varför visar Intune efterlevnadsprincip att min enhet inte har BitLocker aktiverat, även om det är?</span><span class="sxs-lookup"><span data-stu-id="a547f-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="a547f-121">A: inställningen "BitLocker aktiverad" i Intune-efterlevnadsprincipen använder Windows Device Health attestering (DHA)-klienten.</span><span class="sxs-lookup"><span data-stu-id="a547f-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="a547f-122">Den här klienten mäter endast enhetsstatus vid uppstart.</span><span class="sxs-lookup"><span data-stu-id="a547f-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="a547f-123">Så om en enhet inte har startats om eftersom BitLocker-kryptering slutfördes, DHA client service kommer inte att rapportera BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="a547f-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 