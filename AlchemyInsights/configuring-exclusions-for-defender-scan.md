---
title: Konfigurera undantag för sökning i Microsoft Defender ATP
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714353"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="bdffc-102">Konfigurera undantag för sökning i Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="bdffc-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="bdffc-103">I allmänhet kan du utesluta vissa filnamnstillägg och mappplatser från Genomsökningar i Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="bdffc-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="bdffc-104">Du kan också konfigurera undantag för filer som öppnas av vissa processer.</span><span class="sxs-lookup"><span data-stu-id="bdffc-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="bdffc-105">Mer information finns i Konfigurera [och validera](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) undantag baserat på filtillägg och mappplats och konfigurera undantag för filer som öppnas [av processer.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="bdffc-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="bdffc-106">Information om hur du konfigurerar undantag för **Windows Server 2016 och 2019** finns i Konfigurera undantag [för Microsoft Defender Antivirus på Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="bdffc-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="bdffc-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="bdffc-107">**Mac**</span></span>

<span data-ttu-id="bdffc-108">Mer information om undantagstyper som stöds och konfiguration [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) av en lista över undantag för Mac finns i Undantagstyper som stöds och Hur du konfigurerar [en lista över undantag.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="bdffc-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="bdffc-109">**Obs!** Du kan också verifiera undantagslistor med hjälp av testfilen EICAR.</span><span class="sxs-lookup"><span data-stu-id="bdffc-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bdffc-110">Mer information finns i Validera [undantagslistor med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="bdffc-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="bdffc-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="bdffc-111">**Linux**</span></span>

<span data-ttu-id="bdffc-112">Mer information om undantagstyper som stöds och konfiguration [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) av en lista över undantag för Linux finns i Undantagstyper som stöds och Konfigurera och validera undantag för [Microsoft Defender ATP för Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="bdffc-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="bdffc-113">**Obs!** Du kan också verifiera undantagslistor med hjälp av testfilen EICAR.</span><span class="sxs-lookup"><span data-stu-id="bdffc-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bdffc-114">Mer information finns i Validera [undantagslistor med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="bdffc-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 