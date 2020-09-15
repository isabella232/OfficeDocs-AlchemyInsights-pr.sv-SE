---
title: Felsöka problem med att registrera Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658896"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="526e1-102">Felsöka problem med att registrera Windows-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="526e1-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="526e1-103">Granska resurserna nedan för att lösa problemet nu.</span><span class="sxs-lookup"><span data-stu-id="526e1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="526e1-104">Vanliga fel meddelanden och lösnings steg:</span><span class="sxs-lookup"><span data-stu-id="526e1-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="526e1-105">**Det gick inte att installera program varan, 0x80cf4017:** Ditt konto certifikat har upphört att gälla.</span><span class="sxs-lookup"><span data-stu-id="526e1-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="526e1-106">Ladda ner om klient program varu paketet för PC client i Intune-administratörskonsolen.</span><span class="sxs-lookup"><span data-stu-id="526e1-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="526e1-107">Mer information finns i den här dokumentationen.</span><span class="sxs-lookup"><span data-stu-id="526e1-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="526e1-108">**Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:</span><span class="sxs-lookup"><span data-stu-id="526e1-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="526e1-109">Användaren har fler enheter registrerade än enhets gränsen.</span><span class="sxs-lookup"><span data-stu-id="526e1-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="526e1-110">Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra enhetens gräns](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="526e1-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="526e1-111">"Användare kan ansluta enheter till Azure AD" är inställt på "ingen".</span><span class="sxs-lookup"><span data-stu-id="526e1-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="526e1-112">Ange den till alla eller Välj användare.</span><span class="sxs-lookup"><span data-stu-id="526e1-112">Set it to all or select users.</span></span> <span data-ttu-id="526e1-113">Mer information finns i [den här dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="526e1-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="526e1-114">Enheten har redan registrerats av en annan användare.</span><span class="sxs-lookup"><span data-stu-id="526e1-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="526e1-115">Om så är fallet, ta bort enheten från Azure Intune-konsolen eller avregistrera enheten manuellt innan du försöker igen.</span><span class="sxs-lookup"><span data-stu-id="526e1-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="526e1-116">Enheten är Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="526e1-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="526e1-117">Endast Windows 10 Pro, utbildning och företags-SKU: er kan ansluta till Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="526e1-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="526e1-118">Ytterligare resurser för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="526e1-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="526e1-119">Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem.</span><span class="sxs-lookup"><span data-stu-id="526e1-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="526e1-120">Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.</span><span class="sxs-lookup"><span data-stu-id="526e1-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="526e1-121">Granska de här dokumenten för en lista över vanliga fel som kan förhindra registrering och problemlösning för var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="526e1-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="526e1-122">[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="526e1-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
