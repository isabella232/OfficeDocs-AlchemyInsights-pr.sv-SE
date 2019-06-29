---
title: Felsöka problem med att registrera Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353555"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="bb2e8-102">Felsöka problem med att registrera Windows-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb2e8-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="bb2e8-103">Granska resurserna i listan nedan för att åtgärda problemet nu.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bb2e8-104">Vissa vanliga felmeddelanden och stegen:</span><span class="sxs-lookup"><span data-stu-id="bb2e8-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="bb2e8-105">**Går inte att installera programvaran, 0x80cf4017:** Konto-certifikatet har upphört att gälla.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="bb2e8-106">Hämta igen programpaketet PC-klient i Intune-administratörskonsolen.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="bb2e8-107">Läs dokumentationen för mer information.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="bb2e8-108">**Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:</span><span class="sxs-lookup"><span data-stu-id="bb2e8-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="bb2e8-109">Användaren har fler enheter som registrerats än gränsen för enheten.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bb2e8-110">Granska dessa dokument om du vill [Ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra gränsen för enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="bb2e8-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="bb2e8-111">”Användare kan ansluta enheter till Azure AD” anges till ”none”.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="bb2e8-112">Ange alla eller Välj användare.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-112">Set it to all or select users.</span></span> <span data-ttu-id="bb2e8-113">Läs [dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) för mer information.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="bb2e8-114">Enheten är redan registrerats av en annan användare.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="bb2e8-115">Om så är fallet, ta bort enheten från konsolen Azure Intune eller unenroll enheten manuellt innan du försöker igen.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="bb2e8-116">Enheten är Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="bb2e8-117">Endast Windows 10 Pro, utbildning och Enterprise SKU: er kan ansluta till Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="bb2e8-118">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="bb2e8-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bb2e8-119">Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bb2e8-120">Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="bb2e8-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bb2e8-121">Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bb2e8-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="bb2e8-122">[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="bb2e8-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
