---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731257"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4fbde-102">Aktivera BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="4fbde-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="4fbde-103">Intune Endpoint Protection policy kan användas för att konfigurera BitLocker-krypterings inställningar för Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="4fbde-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="4fbde-104">Mer information finns i [Windows 10 (och senare) inställningar för att skydda enheter med Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="4fbde-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="4fbde-105">Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering, som aktive ras utan tillämpning av MDM-principer.</span><span class="sxs-lookup"><span data-stu-id="4fbde-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4fbde-106">Det här kan påverka tillämpningen av policy om icke-standardinställningar konfigureras.</span><span class="sxs-lookup"><span data-stu-id="4fbde-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="4fbde-107">Se följande vanliga frågor för mer information.</span><span class="sxs-lookup"><span data-stu-id="4fbde-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="4fbde-108">Information om hur du felsöker problem med BitLocker finns i [Felsöka BitLocker-principer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="4fbde-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="4fbde-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="4fbde-109">**FAQ**</span></span>

 <span data-ttu-id="4fbde-110">F: vilka versioner av Windows stöder enhets kryptering med Endpoint Protection policy?</span><span class="sxs-lookup"><span data-stu-id="4fbde-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="4fbde-111">A: inställningarna i policyn för Endpoint Protection för Intune implementeras med hjälp av [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="4fbde-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="4fbde-112">Inte alla versioner av Windows har stöd för BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="4fbde-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="4fbde-113">För närvarande stöds följande Windows-utgåvor: Enterprise, Education, Mobile, Mobile Enterprise och Professional (version 1809 och senare).</span><span class="sxs-lookup"><span data-stu-id="4fbde-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="4fbde-114">F: om en enhet redan är krypterad med BitLocker med hjälp av OS-standardinställningarna för krypterings metod och chiffrering (XTS-AES-128) ska en princip med olika inställningar aktive ras automatiskt för åter kryptering av enheten med de nya inställningarna?</span><span class="sxs-lookup"><span data-stu-id="4fbde-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="4fbde-115">S: nej.</span><span class="sxs-lookup"><span data-stu-id="4fbde-115">A: No.</span></span> <span data-ttu-id="4fbde-116">För att använda de nya krypterings inställningarna måste enheten först avkrypteras.</span><span class="sxs-lookup"><span data-stu-id="4fbde-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="4fbde-117">**Obs!** För enheter som är registrerade med autopilot utlöses inte den automatiska krypteringen som skulle inträffa under OOBE förrän Intune-principen utvärderas, vilket gör att de principbaserade inställningarna kan användas i stället för OS-standardinställningarna.</span><span class="sxs-lookup"><span data-stu-id="4fbde-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="4fbde-118">F: om en enhet är krypterad som ett resultat av en Intune-princip kommer den att avkrypteras när den principen tas bort?</span><span class="sxs-lookup"><span data-stu-id="4fbde-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="4fbde-119">A: det går inte att dekryptera de enheter som har kon figurer ATS genom att ta bort krypterings princip.</span><span class="sxs-lookup"><span data-stu-id="4fbde-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="4fbde-120">F: Varför visar policyn för Intune-efterlevnaden att min enhet inte har BitLocker aktiverat, trots att den är?</span><span class="sxs-lookup"><span data-stu-id="4fbde-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="4fbde-121">A: inställningen "BitLocker är aktive rad" i Intune policyn använder DHA-klienten (Windows Device Health attestering).</span><span class="sxs-lookup"><span data-stu-id="4fbde-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4fbde-122">Denna klient mäter bara enhetens tillstånd vid start.</span><span class="sxs-lookup"><span data-stu-id="4fbde-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="4fbde-123">Om en enhet inte har startats om sedan BitLocker-krypteringen har slutförts, rapporterar inte DHA klient tjänsten att aktive ras.</span><span class="sxs-lookup"><span data-stu-id="4fbde-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 