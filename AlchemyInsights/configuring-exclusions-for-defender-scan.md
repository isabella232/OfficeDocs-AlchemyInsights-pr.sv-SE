---
title: Konfigurera undantag för Microsoft Defender ATP sökning
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543703"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="a5c92-102">Konfigurera undantag för Microsoft Defender ATP sökning</span><span class="sxs-lookup"><span data-stu-id="a5c92-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="a5c92-103">I allmänhet kan du utesluta vissa filnamnstillägg och mappplatser från Microsoft Defender ATP genomsökningar.</span><span class="sxs-lookup"><span data-stu-id="a5c92-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="a5c92-104">Du kan också konfigurera undantag för filer som öppnas av vissa processer.</span><span class="sxs-lookup"><span data-stu-id="a5c92-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="a5c92-105">Mer information finns i Konfigurera och validera undantag baserat på [filnamnstillägg](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) och mappplats och Konfigurera undantag för [filer som öppnas med processer.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a5c92-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="a5c92-106">Information om hur du konfigurerar Windows Server 2016 för och **2019** finns i [Microsoft Defender Antivirus på Server Windows undantag.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a5c92-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="a5c92-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="a5c92-107">**Mac**</span></span>

<span data-ttu-id="a5c92-108">Mer information om undantagstyper som stöds och konfiguration [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) av en lista över undantag för Mac finns i Undantagstyper som stöds och Konfigurera [en lista över undantag.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="a5c92-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="a5c92-109">**Obs!** Du kan också verifiera undantagslistor med hjälp av testfilen EICAR.</span><span class="sxs-lookup"><span data-stu-id="a5c92-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a5c92-110">Mer information finns i [Validera undantagslistor med EICAR-testfilen](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="a5c92-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="a5c92-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="a5c92-111">**Linux**</span></span>

<span data-ttu-id="a5c92-112">Mer information om undantagstyper som stöds och konfiguration [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) av en lista över undantag för Linux finns i [Undantagstyper](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)som stöds och Konfigurera och validera undantag för Microsoft Defender ATP för Linux.</span><span class="sxs-lookup"><span data-stu-id="a5c92-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="a5c92-113">**Obs!** Du kan också verifiera undantagslistor med hjälp av testfilen EICAR.</span><span class="sxs-lookup"><span data-stu-id="a5c92-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a5c92-114">Mer information finns i [Validera undantagslistor med EICAR-testfilen](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="a5c92-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 