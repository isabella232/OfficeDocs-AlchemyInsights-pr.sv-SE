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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708980"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="856db-102">Felsöka problem med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="856db-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="856db-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="856db-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="856db-104">Några vanliga felmeddelanden och lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="856db-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="856db-105">**Enhetens änd cap har nåtts** Användaren har fler enheter registrerade än enhetsgränsen.</span><span class="sxs-lookup"><span data-stu-id="856db-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="856db-106">Granska dessa dokument om [du vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="856db-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="856db-107">**Den här tjänsten stöds inte. Ingen registreringspolicy:** Apple Push-aviseringstjänsten (APNS) måste konfigureras eller förnyas.</span><span class="sxs-lookup"><span data-stu-id="856db-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="856db-108">I [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finns anvisningar om hur du gör det.</span><span class="sxs-lookup"><span data-stu-id="856db-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="856db-109">**Användarlicenstyp ogiltig eller användarnamnet identifieras inte:** Användaren måste vara tilldelad en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="856db-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="856db-110">Granska de här dokumenten om du vill tilldela en licens via: [Administrationscenter för Office](https://docs.microsoft.com/intune/licenses-assign) [eller Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="856db-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="856db-111">Ytterligare resurser som kan hjälpa dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="856db-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="856db-112">Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem.</span><span class="sxs-lookup"><span data-stu-id="856db-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="856db-113">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="856db-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="856db-114">I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [felsökningsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="856db-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="856db-115">[Lär dig hur du registrerar iOS-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="856db-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

