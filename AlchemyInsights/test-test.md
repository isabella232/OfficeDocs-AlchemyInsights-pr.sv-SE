---
title: Termer som saknas i SharePoint Online term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053531"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="2811b-102">Aktivera BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="2811b-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="2811b-103">Intune Endpoint Protection-principen kan användas för att konfigurera Boitlocker krypteringsinställningar för Windows-enheter som beskrivs i: windows10 (och senare) inställningar för att skydda enheter med hjälp av Intune</span><span class="sxs-lookup"><span data-stu-id="2811b-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="2811b-104">Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering som utlöses utan tillämpning av MDM-principen.</span><span class="sxs-lookup"><span data-stu-id="2811b-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="2811b-105">Detta kan påverka tillämpningen av principen om icke-standardinställningar har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="2811b-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="2811b-106">Se FAQ för mer information.</span><span class="sxs-lookup"><span data-stu-id="2811b-106">See FAQ for more detail.</span></span>


<span data-ttu-id="2811b-107">FAQ  Q: vilka utgåvor av Windows stöder enhetskryptering med hjälp av Endpoint Protection-principen?</span><span class="sxs-lookup"><span data-stu-id="2811b-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="2811b-108"> A: inställningarna i Intune Endpoint Protection-principen implementeras med hjälp av BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="2811b-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="2811b-109">Inte alla utgåvor eller build-versioner av Windows stöder BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="2811b-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="2811b-110">På denna tid Windows upplagor: företag; Education, Mobile, Mobile Enterprise och Professional (från build 1809 och framåt) stöds.</span><span class="sxs-lookup"><span data-stu-id="2811b-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="2811b-111">F: om en enhet redan är krypterad med BitLocker med hjälp av OS standardinställningarna för krypteringsmetod och cipher styrka (XTS-AES-128) kommer att tillämpa en princip med olika inställningar automatiskt utlösa Omkryptering av enheten med de nya inställningarna?</span><span class="sxs-lookup"><span data-stu-id="2811b-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="2811b-112">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="2811b-112">A: No.</span></span> <span data-ttu-id="2811b-113">För att kunna tillämpa de nya krypteringsinställningarna måste enheten först dekrypteras.</span><span class="sxs-lookup"><span data-stu-id="2811b-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="2811b-114">För enheter som registreras med autopilot aktiveras inte den automatiska kryptering som skulle inträffa under OOBE förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar kan användas i stället för OS-standardvärdena</span><span class="sxs-lookup"><span data-stu-id="2811b-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="2811b-115">F om en enhet krypteras som ett resultat av tillämpningen av Intune-principen dekrypteras när principen tas bort?</span><span class="sxs-lookup"><span data-stu-id="2811b-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="2811b-116">S: borttagning av krypteringsrelaterade principer resulterar inte i dekryptering av enheter som har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="2811b-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="2811b-117">F: Varför visar Intune efterlevnadsprincip att min enhet inte har "BitLocker aktiverat" men det är?</span><span class="sxs-lookup"><span data-stu-id="2811b-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="2811b-118">A: inställningen "BitLocker aktiverad" i Intune efterlevnadsprincip använder Windows Device Health attestering (DHA)-klienten.</span><span class="sxs-lookup"><span data-stu-id="2811b-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="2811b-119">Den här klienten mäter endast enhetsstatus vid uppstart.</span><span class="sxs-lookup"><span data-stu-id="2811b-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="2811b-120">Så om en enhet inte har startats om eftersom BitLocker-kryptering slutfördes kommer inte DHA client service att rapportera BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="2811b-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>