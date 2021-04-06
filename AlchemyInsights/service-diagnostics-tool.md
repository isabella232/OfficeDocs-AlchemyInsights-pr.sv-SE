---
title: Verktyget Tjänstdiagnostik för Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596046"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="ee011-102">Verktyget Tjänstdiagnostik för Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="ee011-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="ee011-103">Windows Virtual Desktop (WVD) innehåller ett diagnostikverktyg som gör att administratörer kan identifiera fel i ett enda gränssnitt.</span><span class="sxs-lookup"><span data-stu-id="ee011-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="ee011-104">Det här verktyget loggar diagnosrelaterad information när WVD används av någon som tilldelats en WVD-roll.</span><span class="sxs-lookup"><span data-stu-id="ee011-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="ee011-105">Varje logg innehåller information om WVD-rollen som ingår i aktiviteten, felmeddelanden som visas under sessionen och information om klientorganisationen och användaren.</span><span class="sxs-lookup"><span data-stu-id="ee011-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="ee011-106">Azure-logganalys kan konfigureras för att registrera aktivitetsloggen som skapats av diagnostikverktyget genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="ee011-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="ee011-107">Skapa en arbetsyta för logganalys med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) [eller Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="ee011-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="ee011-108">[Anslut Windows-datorer till Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="ee011-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="ee011-109">Hämta Arbetsyte-ID och primärnyckel för arbetsytan.</span><span class="sxs-lookup"><span data-stu-id="ee011-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="ee011-110">Installationsguiden behöver den här informationen för att kunna konfigurera agenten på rätt sätt och för att säkerställa att den kan kommunicera med Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="ee011-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="ee011-111">[Skicka diagnostikdata till arbetsytan](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="ee011-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="ee011-112">Du kan push-diagnostikdata från WVD-klienten till logganalysen för arbetsytan.</span><span class="sxs-lookup"><span data-stu-id="ee011-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="ee011-113">[Identifiera och diagnostisera](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problem som är interna eller externa i relation till WVD.</span><span class="sxs-lookup"><span data-stu-id="ee011-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="ee011-114">Mer information om hur du konfigurerar tjänstdiagnostikverktyget för WVD finns i Använda logganalys för diagnostikfunktionen.</span><span class="sxs-lookup"><span data-stu-id="ee011-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>