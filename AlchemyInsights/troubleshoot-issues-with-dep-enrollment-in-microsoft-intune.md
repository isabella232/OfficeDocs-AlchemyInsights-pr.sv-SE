---
title: Felsöka problem med DEP-registrering i Microsoft Intune
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
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708728"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="51c2e-102">Felsöka problem med DEP-registrering i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="51c2e-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="51c2e-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="51c2e-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="51c2e-104">Om DEP-enheten inte kan registrera och MFA (Multi-Factor Authentication) är aktiverat inaktiverar du MFA.</span><span class="sxs-lookup"><span data-stu-id="51c2e-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="51c2e-105">För närvarande stöds inte MFA för DEP-registrering</span><span class="sxs-lookup"><span data-stu-id="51c2e-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="51c2e-106">Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem.</span><span class="sxs-lookup"><span data-stu-id="51c2e-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="51c2e-107">Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="51c2e-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="51c2e-108">I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [felsökningsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="51c2e-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="51c2e-109">[Läs mer om program för enhetsregistrering.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="51c2e-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
