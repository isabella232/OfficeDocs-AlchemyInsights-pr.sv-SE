---
title: Problem med att installera Microsoft Defender på Mac eller Linux
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539698"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="d7387-102">Problem med att installera Microsoft Defender på Mac eller Linux</span><span class="sxs-lookup"><span data-stu-id="d7387-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="d7387-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="d7387-103">**Mac**</span></span>

- <span data-ttu-id="d7387-104">Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Mac.</span><span class="sxs-lookup"><span data-stu-id="d7387-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="d7387-105">Mer information finns i Så [här installerar du Microsoft Defender ATP för Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="d7387-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="d7387-106">Granska informationen i filen: "/Bibliotek/Loggar/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="d7387-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="d7387-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="d7387-107">**Linux**</span></span>

- <span data-ttu-id="d7387-108">Se till att systemkraven uppfylls innan du installerar Microsoft Defender ATP för Linux.</span><span class="sxs-lookup"><span data-stu-id="d7387-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="d7387-109">Mer information finns i [Så här installerar du MDATP för Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="d7387-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="d7387-110">Kontrollera att MDATP körs i Installationen [misslyckades.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="d7387-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="d7387-111">Information om hur du felsöker och löser problem om tjänsten inte körs finns i Anvisningar för att felsöka [om mdatp-tjänsten inte körs.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="d7387-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="d7387-112">Information om hur du kontrollerar klientkonfigurationen, som verifierar hälsotillståndet för produkten och kör ett identifieringstest på textfilen EICAR finns i [Klientkonfiguration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="d7387-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="d7387-113">**Obs!** En lista över filsystem som stöds för aktivitet vid åtkomst finns i [Microsoft Defender ATP för Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="d7387-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>