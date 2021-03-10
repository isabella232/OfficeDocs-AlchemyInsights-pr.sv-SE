---
title: Konfigurera och validera undantag för MDATP på en Linux-dator
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696071"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="345f2-102">Konfigurera och validera undantag för MDATP på en Linux-dator</span><span class="sxs-lookup"><span data-stu-id="345f2-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="345f2-103">Du kan utesluta vissa filer, mappar, processer och process öppna filer från MDATP-skanningar.</span><span class="sxs-lookup"><span data-stu-id="345f2-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="345f2-104">Undantag förhindrar felaktig identifiering av programvara och filer som är unika eller anpassade för din organisation.</span><span class="sxs-lookup"><span data-stu-id="345f2-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="345f2-105">Undantag bidrar också till att minimera prestandaproblem som orsakas av MDATP.</span><span class="sxs-lookup"><span data-stu-id="345f2-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="345f2-106">Mer information finns i Konfigurera [och validera undantag för MDATP för Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="345f2-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="345f2-107">Undantagen som beskrivs i den här artikeln gäller inte för andra funktioner i MDATP för Linux, inklusive slutpunktsidentifiering och svar (EDR).</span><span class="sxs-lookup"><span data-stu-id="345f2-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="345f2-108">Filer som du utesluter med hjälp av de metoder som beskrivs i den här artikeln kan fortfarande utlösa EDR-aviseringar och andra identifieringsfunktioner.</span><span class="sxs-lookup"><span data-stu-id="345f2-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
