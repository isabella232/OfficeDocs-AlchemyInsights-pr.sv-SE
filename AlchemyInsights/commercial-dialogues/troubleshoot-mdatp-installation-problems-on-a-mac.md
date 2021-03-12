---
title: Felsöka problem med MDATP-installationen på en Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749767"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="b01b1-102">Felsöka problem med MDATP-installationen på en Mac</span><span class="sxs-lookup"><span data-stu-id="b01b1-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="b01b1-103">Om manuell installation misslyckas **visas** följande fel på sidan Sammanfattning av installationsguiden:</span><span class="sxs-lookup"><span data-stu-id="b01b1-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="b01b1-104">"Ett fel uppstod under installationen.</span><span class="sxs-lookup"><span data-stu-id="b01b1-104">"An error occurred during installation.</span></span> <span data-ttu-id="b01b1-105">Installationsprogrammet påträffade ett fel som orsakade att installationen misslyckades.</span><span class="sxs-lookup"><span data-stu-id="b01b1-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="b01b1-106">Kontakta programvarutillverkaren för att få hjälp."</span><span class="sxs-lookup"><span data-stu-id="b01b1-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="b01b1-107">För MDM-distributioner visar sidan också ett allmänt installationsfel.</span><span class="sxs-lookup"><span data-stu-id="b01b1-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="b01b1-108">Även om vi inte visar exakta fel för slutanvändare så sparar vi en loggfil med installationsstatus i **/Bibliotek/Loggar/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="b01b1-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="b01b1-109">Varje installationssession läggs till i den här loggfilen.</span><span class="sxs-lookup"><span data-stu-id="b01b1-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="b01b1-110">Om du bara vill mata ut den senaste installationssessionen använder du `sed` .</span><span class="sxs-lookup"><span data-stu-id="b01b1-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="b01b1-111">Mer information finns i [Felsöka installationsproblem för Microsoft Defender ATP för Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="b01b1-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
