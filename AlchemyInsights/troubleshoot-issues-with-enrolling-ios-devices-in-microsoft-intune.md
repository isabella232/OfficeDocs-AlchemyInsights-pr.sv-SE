---
title: Felsöka problem med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669266"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2476f-102">Felsöka problem med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2476f-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2476f-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="2476f-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2476f-104">Vanliga fel meddelanden och lösnings steg:</span><span class="sxs-lookup"><span data-stu-id="2476f-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2476f-105">**Höljet har nåtts** Användaren har fler enheter registrerade än enhets gränsen.</span><span class="sxs-lookup"><span data-stu-id="2476f-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2476f-106">Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra enhetens gräns](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2476f-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2476f-107">**Den här tjänsten stöds inte. Ingen registrerings princip:** Apple Push Notification Service (APN) måste konfigureras eller förnyas.</span><span class="sxs-lookup"><span data-stu-id="2476f-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2476f-108">Läs [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för anvisningar om hur du gör det.</span><span class="sxs-lookup"><span data-stu-id="2476f-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2476f-109">**Användar licens typen är ogiltig eller användar namnet känns inte igen:** Användaren måste tilldelas en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="2476f-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2476f-110">Granska dessa dokument om du vill tilldela en licens via: [administrations Center för Office](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2476f-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2476f-111">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="2476f-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2476f-112">Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem.</span><span class="sxs-lookup"><span data-stu-id="2476f-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2476f-113">Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="2476f-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2476f-114">Granska de här dokumenten för en lista över vanliga fel som kan förhindra registrering och problemlösning för var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2476f-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2476f-115">[Lär dig hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2476f-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

