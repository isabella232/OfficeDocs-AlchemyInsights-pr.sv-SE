---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492232"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9c8b1-102">Felsöka problem med att registrera Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9c8b1-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9c8b1-103">Granska resurserna i listan nedan för att åtgärda problemet nu.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9c8b1-104">Vissa vanliga problem och stegen:</span><span class="sxs-lookup"><span data-stu-id="9c8b1-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9c8b1-p101">**Enhet krypteras inte fel i företagets Portal:** Nyare versioner av Android, särskilt från och med v7.0, kräver en start-kod för att kontrollera att enheten är helt krypterad. Gemensamma lösningar är att aktivera en start-PIN-kod eller helt kryptera enheten. Granska [dokumentet](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="9c8b1-p102">**Enheter misslyckas att checka in med tjänsten Intune eller visas som ”ohälsosamt” i Intune-administratörskonsolen:** Vissa Samsung 4.4 och 5.5 enheter kan inte checka in i tjänsten. Det finns 3 möjliga lösningar på problemet:</span><span class="sxs-lookup"><span data-stu-id="9c8b1-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="9c8b1-110">Öppna appen Intune-företagsportal som kommer automatiskt att starta en enhetssynkronisering manuellt.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="9c8b1-111">Uppdatera enheten till Android 6.0 eller senare.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="9c8b1-p103">Inaktivera Samsung Smart Manager från att hantera Intune-företagsportal. Granska [dokumentet](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) för mer information om dessa problem och lösningar.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="9c8b1-p104">**Ogiltig användare licens typ** eller **användare namn inte identifieras fel:** användaren måste tilldelas en Intune eller EMS-licens. Granska dessa dokument om du vill tilldela en licens till: Office Admin Center eller Azure portal.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="9c8b1-116">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="9c8b1-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9c8b1-p105">Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/en-us/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9c8b1-119">Granska [dokumentet](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som förhindrar registrering och lösningar till varje.</span><span class="sxs-lookup"><span data-stu-id="9c8b1-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="9c8b1-120">[Lär dig att registrera Android-enheter i Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="9c8b1-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

