---
title: Felsöka problem med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823481"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="feefb-102">Felsöka problem med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="feefb-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="feefb-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="feefb-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="feefb-104">Några vanliga felmeddelanden och lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="feefb-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="feefb-105">**Enhetens änd cap har nåtts** Användaren har fler enheter registrerade än enhetsgränsen.</span><span class="sxs-lookup"><span data-stu-id="feefb-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="feefb-106">Läs dessa dokument om du [vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="feefb-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="feefb-107">**Den här tjänsten stöds inte. Ingen registreringspolicy:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas.</span><span class="sxs-lookup"><span data-stu-id="feefb-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="feefb-108">Läs [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för anvisningar om hur du gör det.</span><span class="sxs-lookup"><span data-stu-id="feefb-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="feefb-109">**Användarlicenstyp Ogiltig eller Användarnamnet har inte identifierats:** Användaren måste tilldelas en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="feefb-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="feefb-110">Läs dessa dokument om du vill tilldela en licens via: [Administrationscenter för Office](https://docs.microsoft.com/intune/licenses-assign) [eller Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="feefb-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="feefb-111">Ytterligare resurser som kan hjälpa dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="feefb-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="feefb-112">Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel.</span><span class="sxs-lookup"><span data-stu-id="feefb-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="feefb-113">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="feefb-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="feefb-114">I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökningsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="feefb-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="feefb-115">[Lär dig hur du registrerar iOS-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="feefb-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

