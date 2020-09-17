---
title: Felsöka problem med DATAEXEKVERINGSSKYDD i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797314"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="d97f7-102">Felsöka problem med DATAEXEKVERINGSSKYDD i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d97f7-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="d97f7-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="d97f7-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="d97f7-104">Om DEP-enheten inte kan registrera och MFA (multifaktorautentisering) är aktive rad måste du inaktivera MFA.</span><span class="sxs-lookup"><span data-stu-id="d97f7-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="d97f7-105">För närvarande stöds inte för MFA-registrering</span><span class="sxs-lookup"><span data-stu-id="d97f7-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="d97f7-106">Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem.</span><span class="sxs-lookup"><span data-stu-id="d97f7-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d97f7-107">Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="d97f7-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="d97f7-108">Granska dessa dokument för en lista över vanliga fel som kan förhindra registrering och upplösningar på var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d97f7-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="d97f7-109">[Läs mer om programmet för enhets registrering](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="d97f7-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
