---
title: Felsöka problem med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689972"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ecc14-102">Felsöka problem med registrering av Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ecc14-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ecc14-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="ecc14-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ecc14-104">Några vanliga problem och problemlösning:</span><span class="sxs-lookup"><span data-stu-id="ecc14-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ecc14-105">**Enheten är inte krypterad fel i företags portalen:** Nyare versioner av Android, särskilt från och med v 7.0, kräver ett start program för att kontrol lera att enheten är fullständigt krypterad.</span><span class="sxs-lookup"><span data-stu-id="ecc14-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ecc14-106">Vanliga lösningar är att aktivera en start-PIN-kod eller helt kryptera enheten.</span><span class="sxs-lookup"><span data-stu-id="ecc14-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ecc14-107">Granska [det här dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.</span><span class="sxs-lookup"><span data-stu-id="ecc14-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ecc14-108">**Enheter kan inte checka in med Intune-tjänsten eller Visa som "ohälsosamy" i Intune-administratörskonsolen:** Vissa Samsung 4,4-och 5,5-enheter kanske inte checkar in tjänsten.</span><span class="sxs-lookup"><span data-stu-id="ecc14-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ecc14-109">Det finns tre möjliga lösningar på det här problemet:</span><span class="sxs-lookup"><span data-stu-id="ecc14-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ecc14-110">Öppna programmet Intune-företagsportalsappen manuellt, som automatiskt initierar en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="ecc14-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ecc14-111">Uppdatera enheten till Android 6,0 eller högre.</span><span class="sxs-lookup"><span data-stu-id="ecc14-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ecc14-112">Inaktivera den smarta hanteraren för Samsung från att hantera Intune-företagsportalsappen.</span><span class="sxs-lookup"><span data-stu-id="ecc14-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ecc14-113">Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) om du vill ha mer information om dessa problem och lösningar.</span><span class="sxs-lookup"><span data-stu-id="ecc14-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ecc14-114">**Användar licens typen är ogiltig** eller **användar namnet känns inte igen:** användaren måste tilldelas en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="ecc14-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ecc14-115">Granska dessa dokument om du vill tilldela en licens via: administrations Center för Office eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ecc14-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ecc14-116">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="ecc14-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ecc14-117">Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem.</span><span class="sxs-lookup"><span data-stu-id="ecc14-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ecc14-118">Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="ecc14-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ecc14-119">Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som kan förhindra registrering och upplösningar till var och en.</span><span class="sxs-lookup"><span data-stu-id="ecc14-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ecc14-120">[Lär dig att registrera Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ecc14-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
