---
title: Felsöka problem med att registrera iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507021"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="99247-102">Felsöka problem med att registrera iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="99247-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="99247-103">Granska resurserna som anges nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="99247-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="99247-104">Några vanliga felmeddelanden och Lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="99247-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="99247-105">**Enhets locket har uppnåtts** Användaren har fler enheter registrerade än enhets gränsen.</span><span class="sxs-lookup"><span data-stu-id="99247-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="99247-106">Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [ändra enhets gränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="99247-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="99247-107">**Den här tjänsten stöds inte. Ingen registreringsprincip:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas.</span><span class="sxs-lookup"><span data-stu-id="99247-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="99247-108">Läs igenom [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för instruktioner om hur du gör det.</span><span class="sxs-lookup"><span data-stu-id="99247-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="99247-109">**Användarlicenstyp ogiltig eller användarnamn känns inte igen:** Användaren måste tilldelas en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="99247-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="99247-110">Granska dessa dokument för att tilldela en licens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="99247-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="99247-111">Ytterligare resurser som hjälper dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="99247-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="99247-112">Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel.</span><span class="sxs-lookup"><span data-stu-id="99247-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="99247-113">Läs igenom [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="99247-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="99247-114">Granska de här dokumenten för en lista över vanliga fel som förhindrar registrering och upplösningar för varje: [felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)av dokument.</span><span class="sxs-lookup"><span data-stu-id="99247-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="99247-115">[Lär dig hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="99247-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

