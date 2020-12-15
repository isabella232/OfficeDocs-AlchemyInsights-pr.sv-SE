---
title: Service Diagnostics Tool för Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680233"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="867aa-102">Service Diagnostics Tool för Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="867aa-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="867aa-103">Windows Virtual Desktop (WVD) erbjuder ett diagnostikverktyg som låter administratörer identifiera fel genom ett enda gränssnitt.</span><span class="sxs-lookup"><span data-stu-id="867aa-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="867aa-104">Det här verktyget loggar diagnostikinformation-relaterad information när WVD används av någon som tilldelats en WVD-roll.</span><span class="sxs-lookup"><span data-stu-id="867aa-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="867aa-105">Varje logg innehåller information om den WVD rollen som är involverad i aktiviteten, de fel meddelanden som visas under sessionen samt uppgifter om klient organisationen och användaren.</span><span class="sxs-lookup"><span data-stu-id="867aa-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="867aa-106">Azure Log Analytics kan konfigureras för att fånga in aktivitets loggen som skapas av diagnostikverktyget.</span><span class="sxs-lookup"><span data-stu-id="867aa-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="867aa-107">Så här gör du:</span><span class="sxs-lookup"><span data-stu-id="867aa-107">Here's how:</span></span>

1. <span data-ttu-id="867aa-108">Skapa en logganalys-arbetsyta med [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="867aa-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="867aa-109">[Anslut Windows-datorer till Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="867aa-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="867aa-110">Hämta arbetsyte-ID och primärt för arbets ytan.</span><span class="sxs-lookup"><span data-stu-id="867aa-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="867aa-111">Installations guiden behöver den här informationen för att konfigurera agenten på rätt sätt och för att säkerställa att den kan kommunicera med Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="867aa-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="867aa-112">[Pusha diagnostikdata till din arbets yta](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="867aa-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="867aa-113">Du kan skicka diagnos data från din WVD-klient till logg analys för arbets ytan.</span><span class="sxs-lookup"><span data-stu-id="867aa-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="867aa-114">[Identifiera och diagnostisera problem](https://go.microsoft.com/fwlink/?linkid=2128338) som är interna eller externa i relation till WVD.</span><span class="sxs-lookup"><span data-stu-id="867aa-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="867aa-115">Mer information om hur du konfigurerar verktyget för WVD finns i [använda logg analys för funktionen diagnostik](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="867aa-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
