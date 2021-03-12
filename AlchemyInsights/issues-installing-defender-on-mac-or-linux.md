---
title: Problem med installationen av Microsoft Defender på Mac eller Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714317"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="22cac-102">Problem med installationen av Microsoft Defender på Mac eller Linux</span><span class="sxs-lookup"><span data-stu-id="22cac-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="22cac-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="22cac-103">**Mac**</span></span>

- <span data-ttu-id="22cac-104">Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Mac.</span><span class="sxs-lookup"><span data-stu-id="22cac-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="22cac-105">Mer information finns i Installera [Microsoft Defender ATP för Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="22cac-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="22cac-106">Granska informationen i filen: "/Bibliotek/Loggar/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="22cac-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="22cac-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="22cac-107">**Linux**</span></span>

- <span data-ttu-id="22cac-108">Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Linux.</span><span class="sxs-lookup"><span data-stu-id="22cac-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="22cac-109">Mer information finns i Installera [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="22cac-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="22cac-110">Kontrollera att MDATP-tjänsten körs genom att gå till [Installationen misslyckades.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="22cac-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="22cac-111">Information om hur du felsöker och löser problem om tjänsten inte körs finns i Anvisningar för att felsöka [om mdatp-tjänsten inte körs.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="22cac-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="22cac-112">Instruktioner för hur du kontrollerar klientkonfigurationen, som verifierar hälsotillståndet för produkten och kör ett identifieringstest på TEXTfilen EICAR, finns i [Klientkonfiguration.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="22cac-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="22cac-113">**Obs!** En lista över filsystem som stöds för aktivitet vid åtkomst finns i [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="22cac-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>