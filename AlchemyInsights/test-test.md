---
title: Termer saknas i SharePoint Online term lagrings plats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750469"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="58d17-102">Aktivera BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="58d17-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="58d17-103">Intune Endpoint Protection policy kan användas för att konfigurera Boitlocker krypterings inställningar för Windows-enheter enligt beskrivningen i: windows10 (och senare) inställningar för att skydda enheter med Intune</span><span class="sxs-lookup"><span data-stu-id="58d17-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="58d17-104">Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering som aktive ras utan tillämpning av MDM-princip.</span><span class="sxs-lookup"><span data-stu-id="58d17-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="58d17-105">Det här kan påverka tillämpningen av policy om icke-standardinställningar konfigureras.</span><span class="sxs-lookup"><span data-stu-id="58d17-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="58d17-106">Se vanliga frågor för mer information.</span><span class="sxs-lookup"><span data-stu-id="58d17-106">See FAQ for more detail.</span></span>


<span data-ttu-id="58d17-107">Vanliga frågor   Q: vilka versioner av Windows stöder enhets kryptering som använder Endpoint Protection policy?</span><span class="sxs-lookup"><span data-stu-id="58d17-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="58d17-108"> A: inställningarna i policyn för Endpoint Protection för Intune implementeras med hjälp av BitLocker-CSP.</span><span class="sxs-lookup"><span data-stu-id="58d17-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="58d17-109">Alla versioner av Windows stöder inte heller BitLocker-CSP: n. 
     </span><span class="sxs-lookup"><span data-stu-id="58d17-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="58d17-110">I den här tiden Windows-utgåvor: Enterprise; Utbildning och mobil telefon, mobil telefon och professionellt stöd (från version 1809).</span><span class="sxs-lookup"><span data-stu-id="58d17-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="58d17-111">F: om en enhet redan är krypterad med BitLocker med hjälp av OS-standardinställningarna för krypterings metod och chiffrering (XTS-AES-128) tillämpas en princip med olika inställningar automatiskt återaktiverar enheten med de nya inställningarna?</span><span class="sxs-lookup"><span data-stu-id="58d17-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="58d17-112">S: nej.</span><span class="sxs-lookup"><span data-stu-id="58d17-112">A: No.</span></span> <span data-ttu-id="58d17-113">För att använda de nya inställningarna för chiffrering måste enheten först dekrypteras.</span><span class="sxs-lookup"><span data-stu-id="58d17-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="58d17-114">Anmärkning för enheter som är registrerade med autopilot en automatisk kryptering som skulle inträffa under OOBE utlöses inte förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar används i stället för OS-standardinställningarna</span><span class="sxs-lookup"><span data-stu-id="58d17-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="58d17-115">F om en enhet är krypterad som ett resultat av en Intune-princip kommer den att avkrypteras när den principen tas bort?</span><span class="sxs-lookup"><span data-stu-id="58d17-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="58d17-116">A: det går inte att dekryptera de enheter som har kon figurer ATS när krypterings relaterad princip tas bort.</span><span class="sxs-lookup"><span data-stu-id="58d17-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="58d17-117">F: Varför visas inte min enhet "BitLocker aktive rad" i Intune policy för efterlevnad?</span><span class="sxs-lookup"><span data-stu-id="58d17-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="58d17-118">A: inställningen "BitLocker är aktive rad" i Intune policyn använder DHA-klienten (Windows Device Health attestering).</span><span class="sxs-lookup"><span data-stu-id="58d17-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="58d17-119">Denna klient mäter bara enhetens tillstånd vid start.</span><span class="sxs-lookup"><span data-stu-id="58d17-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="58d17-120">Om en enhet inte har startats om sedan BitLocker-krypteringen är slutförd, rapporterar inte BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="58d17-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>