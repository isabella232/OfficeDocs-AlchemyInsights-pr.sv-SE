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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507021"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="80fa2-102">Felsöka problem med att registrera iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="80fa2-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="80fa2-103">Granska resurserna i listan nedan för att åtgärda problemet nu.</span><span class="sxs-lookup"><span data-stu-id="80fa2-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="80fa2-104">Vissa vanliga felmeddelanden och stegen:</span><span class="sxs-lookup"><span data-stu-id="80fa2-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="80fa2-105">**Enheten Cap uppnåtts** Användaren har fler enheter som registrerats än gränsen för enheten.</span><span class="sxs-lookup"><span data-stu-id="80fa2-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="80fa2-106">Granska dessa dokument om du vill [Ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra gränsen för enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="80fa2-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="80fa2-107">**Den här tjänsten stöds inte. Ingen registreringsprincip:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas.</span><span class="sxs-lookup"><span data-stu-id="80fa2-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="80fa2-108">Granska [dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för instruktioner om hur du ska göra.</span><span class="sxs-lookup"><span data-stu-id="80fa2-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="80fa2-109">**Felaktig user License eller okänt användarnamn:** Användaren måste tilldelas en Intune eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="80fa2-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="80fa2-110">Granska dessa dokument om du vill tilldela en licens till: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="80fa2-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="80fa2-111">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="80fa2-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="80fa2-112">Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan.</span><span class="sxs-lookup"><span data-stu-id="80fa2-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="80fa2-113">Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="80fa2-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="80fa2-114">Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="80fa2-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="80fa2-115">[Lär dig att registrera iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="80fa2-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

