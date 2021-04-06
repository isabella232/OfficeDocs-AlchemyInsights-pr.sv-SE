---
title: Identifiera problem med virtuellt skrivbord för Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596035"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="ebe8c-102">Identifiera problem med virtuellt skrivbord för Windows</span><span class="sxs-lookup"><span data-stu-id="ebe8c-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="ebe8c-103">Diagnostik för virtuellt skrivbord i Windows använder bara en PowerShell-cmdlet men innehåller många valfria parametrar för att begränsa och isolera problem.</span><span class="sxs-lookup"><span data-stu-id="ebe8c-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="ebe8c-104">Så här kommer du igång:</span><span class="sxs-lookup"><span data-stu-id="ebe8c-104">To get started:</span></span> 

1. <span data-ttu-id="ebe8c-105">Ladda ned och importera Windows Virtual Desktop PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="ebe8c-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="ebe8c-106">Mer information finns i [Windows Virtual Desktop Cmdlets för Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="ebe8c-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="ebe8c-107">Kör följande cmdlet för att logga in på ditt konto:</span><span class="sxs-lookup"><span data-stu-id="ebe8c-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="ebe8c-108">Exempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="ebe8c-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="ebe8c-109">**OBS!** Alla frågor med PowerShell måste innehålla parametrarna -UserName eller -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="ebe8c-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="ebe8c-110">Information om övervakningsfunktioner finns i Använda [logganalys för diagnostikfunktionen.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="ebe8c-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="ebe8c-111">Om du vill filtrera diagnostikaktiviteter efter användare kör du följande cmdlet:</span><span class="sxs-lookup"><span data-stu-id="ebe8c-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="ebe8c-112">Exempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="ebe8c-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="ebe8c-113">Det finns en lista med filter som du kan köra för att diagnostisera problem.</span><span class="sxs-lookup"><span data-stu-id="ebe8c-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="ebe8c-114">Mer information om diagnostiseringsproblem finns i [Identifiera och diagnostisera problem med Windows Virtual Desktop.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="ebe8c-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="ebe8c-115">Mer information om vanliga fel finns i [Vanliga fel senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="ebe8c-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
