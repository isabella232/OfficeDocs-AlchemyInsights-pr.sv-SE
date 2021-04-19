---
title: 'AIP-skanner: installation och konfiguration'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821681"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: installation och konfiguration

**Installera AIP-skannern genom att följa de rekommenderade riktlinjerna:**

1. Om du uppgraderar och inte utför en ren installation kontrollerar du att du har följt riktlinjerna för uppgradering av Azure Information Protection-skannern och för enhetlig etikettklient finns i uppgradera [Azure Information Protection-skannern](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner). [](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Kontrollera att du uppfyller alla krav [för brandväggar och nätverksinfrastruktur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Kontrollera att dina [principer är inställda](https://docs.microsoft.com/azure/information-protection/configure-policy) på automatisk märkning eller har en standardetikett i principen.
4. Se till att den relevanta filtypen har konfigurerats för etikett/skydd enligt beskrivningen i Filtyper som [stöds av Azure Information Protection-klienten.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Om du dessutom vill ändra standardbeteendet följer du de här riktlinjerna: [Ändra standardskyddsnivån för filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontrollera att användarkontot som konfigurerats för att köra skannertjänsten har behörighet att komma åt alla konfigurerade lagringsplatsen.
6. Om du fortfarande har problem kan du exportera skannerloggarna och lägga till dem i ditt supportärenden.

**Exportera Azure Information Protection-skannerns loggar**

1. Gå till %localappdata%\Microsoft\MSIP under användarkontexten som kör skannertjänsten.
2. Zippa allt innehåll under MSIP-mappen.
3. Spara loggarna till platsen du valt och bifoga dem till din tjänstbegäran.
4. Du kan också använda [Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Mer information finns i:**
- [Distribuera Azure Information Protection-skannern för att automatiskt klassificera och skydda filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Ange och använda tokenparametern för Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Köra en identifieringscykel och visa rapporter för skannern](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Granska dokumentation om Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Hämta Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
