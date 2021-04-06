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
# <a name="identify-windows-virtual-desktop-issues"></a>Identifiera problem med virtuellt skrivbord för Windows

Diagnostik för virtuellt skrivbord i Windows använder bara en PowerShell-cmdlet men innehåller många valfria parametrar för att begränsa och isolera problem. Så här kommer du igång: 

1. Ladda ned och importera Windows Virtual Desktop PowerShell-modulen. Mer information finns i [Windows Virtual Desktop Cmdlets för Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Kör följande cmdlet för att logga in på ditt konto:
    
    Exempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**OBS!** Alla frågor med PowerShell måste innehålla parametrarna -UserName eller -ActivityID. Information om övervakningsfunktioner finns i Använda [logganalys för diagnostikfunktionen.](https://go.microsoft.com/fwlink/?linkid=2126847)

Om du vill filtrera diagnostikaktiviteter efter användare kör du följande cmdlet:

Exempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Det finns en lista med filter som du kan köra för att diagnostisera problem. Mer information om diagnostiseringsproblem finns i [Identifiera och diagnostisera problem med Windows Virtual Desktop.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Mer information om vanliga fel finns i [Vanliga fel senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
