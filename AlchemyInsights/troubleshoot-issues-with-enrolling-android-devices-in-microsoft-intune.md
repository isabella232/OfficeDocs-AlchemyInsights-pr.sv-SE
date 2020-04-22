---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759638"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="c8ca5-102">Felsöka problem med att registrera Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c8ca5-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="c8ca5-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c8ca5-104">Några vanliga problem och lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="c8ca5-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="c8ca5-105">**Enheten har inte krypterat fel i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver en startlösenkod för att se till att enheten är helt krypterad.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="c8ca5-106">Vanliga lösningar är att aktivera en startstift eller kryptera enheten helt.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="c8ca5-107">Läs [det här dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="c8ca5-108">**Enheter kan inte checka in med Intune-tjänsten eller visas som "Ohälsosam" i Intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in på tjänsten.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="c8ca5-109">Det finns tre möjliga lösningar på problemet:</span><span class="sxs-lookup"><span data-stu-id="c8ca5-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="c8ca5-110">Öppna Intune Company Portal-appen manuellt, som automatiskt initierar en enhetssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="c8ca5-111">Uppdatera enheten till Android 6.0 eller senare.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="c8ca5-112">Inaktivera Samsung Smart Manager från att hantera Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="c8ca5-113">Läs [det här dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) för mer information om dessa frågor och lösningar.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="c8ca5-114">**Fel i användarlicenstypen** Ogiltigt eller **fel som inte känns igen för användarnamn:** Användaren måste tilldelas en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c8ca5-115">Granska dessa dokument för att tilldela en licens via: Office Admin Center eller Azure-portal.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="c8ca5-116">Ytterligare resurser som hjälper dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="c8ca5-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c8ca5-117">Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c8ca5-118">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="c8ca5-119">Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som förhindrar registrering och lösningar till var och en.</span><span class="sxs-lookup"><span data-stu-id="c8ca5-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="c8ca5-120">[Läs om hur du registrerar Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="c8ca5-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
