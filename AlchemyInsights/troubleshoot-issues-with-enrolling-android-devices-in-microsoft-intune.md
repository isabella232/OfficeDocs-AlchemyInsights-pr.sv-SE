---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709016"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="92634-102">Felsöka problem med att registrera Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="92634-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="92634-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="92634-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="92634-104">Några vanliga problem och lösningssteg:</span><span class="sxs-lookup"><span data-stu-id="92634-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="92634-105">**Fel vid enhetskrypterad kommunikation i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver ett lösenord för start för att kontrollera att enheten är fullständigt krypterad.</span><span class="sxs-lookup"><span data-stu-id="92634-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="92634-106">Vanliga lösningar är att aktivera en start-PIN eller kryptera enheten helt.</span><span class="sxs-lookup"><span data-stu-id="92634-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="92634-107">Mer information [finns i](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) det här dokumentet.</span><span class="sxs-lookup"><span data-stu-id="92634-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="92634-108">**Enheter kan inte checka in med Intune-tjänsten eller visas som "Ej fel" i intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in tjänsten.</span><span class="sxs-lookup"><span data-stu-id="92634-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="92634-109">Det finns tre möjliga lösningar på det här problemet:</span><span class="sxs-lookup"><span data-stu-id="92634-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="92634-110">Öppna appen Intune-företagsportal manuellt, som automatiskt initierar en enhetssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="92634-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="92634-111">Uppdatera enheten till Android 6.0 eller senare.</span><span class="sxs-lookup"><span data-stu-id="92634-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="92634-112">Inaktivera Samsungs Smart Manager från att hantera Intune-företagsportalen.</span><span class="sxs-lookup"><span data-stu-id="92634-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="92634-113">I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) finns mer information om dessa problem och lösningar.</span><span class="sxs-lookup"><span data-stu-id="92634-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="92634-114">**Felet Ogiltig användarlicenstyp** **eller Användarnamnet identifieras inte:** Användaren måste tilldelas en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="92634-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="92634-115">Granska dessa dokument för att tilldela en licens via: Administrationscenter för Office eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="92634-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="92634-116">Ytterligare resurser som kan hjälpa dig att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="92634-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="92634-117">Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem.</span><span class="sxs-lookup"><span data-stu-id="92634-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="92634-118">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="92634-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="92634-119">I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en.</span><span class="sxs-lookup"><span data-stu-id="92634-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="92634-120">[Lär dig hur du registrerar Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="92634-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
