---
title: Felsöka problem med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830960"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9b088-102">Felsöka problem med registrering av Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9b088-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9b088-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="9b088-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9b088-104">Några vanliga problem och lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="9b088-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9b088-105">**Felmeddelande om att enheten inte är krypterad i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver ett lösenord för start så att enheten är fullständigt krypterad.</span><span class="sxs-lookup"><span data-stu-id="9b088-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="9b088-106">Vanliga lösningar är att aktivera en startkod eller kryptera enheten helt och hållet.</span><span class="sxs-lookup"><span data-stu-id="9b088-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="9b088-107">Mer information [finns i](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) det här dokumentet.</span><span class="sxs-lookup"><span data-stu-id="9b088-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="9b088-108">**Enheter kan inte checka in med Intune-tjänsten eller visas som "Ej fel" i Intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in tjänsten.</span><span class="sxs-lookup"><span data-stu-id="9b088-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="9b088-109">Det finns 3 möjliga lösningar på det här problemet:</span><span class="sxs-lookup"><span data-stu-id="9b088-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="9b088-110">Öppna appen Intune Company Portal manuellt, som automatiskt initierar en enhetssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="9b088-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="9b088-111">Uppdatera enheten till Android 6.0 eller senare.</span><span class="sxs-lookup"><span data-stu-id="9b088-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="9b088-112">Inaktivera Samsung Smart Manager från att hantera Intune-företagsportalen.</span><span class="sxs-lookup"><span data-stu-id="9b088-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="9b088-113">Läs [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) om du vill ha mer information om dessa problem och lösningar.</span><span class="sxs-lookup"><span data-stu-id="9b088-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="9b088-114">**Felet Ogiltig användarlicenstyp** **eller Namn identifieras inte:** Användaren måste tilldelas en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="9b088-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9b088-115">Läs dessa dokument om du vill tilldela en licens via: Administrationscenter för Office eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9b088-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="9b088-116">Ytterligare resurser som kan hjälpa dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="9b088-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9b088-117">Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel.</span><span class="sxs-lookup"><span data-stu-id="9b088-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9b088-118">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="9b088-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9b088-119">I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en.</span><span class="sxs-lookup"><span data-stu-id="9b088-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="9b088-120">[Lär dig hur du registrerar Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="9b088-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
