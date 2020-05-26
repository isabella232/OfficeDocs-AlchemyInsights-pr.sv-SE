---
title: 'AIP-skanner: installation och konfiguration'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358567"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanner: installation och konfiguration

**Så här installerar du AIP-skannern:**

1. Om du uppgraderar och inte utför en ren installation, se till att du har följt riktlinjerna för [uppgradering av Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) och för enhetlig märkning klient, se uppgradera Azure Information Protection [scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontrollera att du uppfyller alla krav på [brandväggar och inställningar för nätverksinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Kontrollera att dina [principer är inställda på](https://docs.microsoft.com/azure/information-protection/configure-policy) automatisk märkning eller har en standardetikett i principen.
4. Kontrollera att den relevanta filtypen är konfigurerad för etikett/skydd enligt beskrivningen i Filtyper som [stöds av Azure Information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Om du vill ändra standardbeteendet följer du dessutom dessa riktlinjer: [Ändra standardskyddsnivån för filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontrollera att användarkontot som konfigurerats för att köra skannertjänsten har behörighet att komma åt alla konfigurerade databaser.
6. Om du fortfarande har problem kan du exportera skannerloggarna och lägga till dem i supportbiljetten.

**Exportera Azure Information Protection Scanner-loggar**

1. Navigera till %localappdata%\Microsoft\MSIP under användarkontexten som kör skannertjänsten.
2. Zip allt innehåll under MSIP-mappen.
3. Spara loggarna till ditt val av plats och bifoga dem till din servicebegäran.
4. Du kan också använda [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Mer information finns i:**
- [Distribuera Azure Information Protection-skannern för att automatiskt klassificera och skydda filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Ange och använda parametern Token för Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Kör en identifieringscykel och visa rapporter för skannern](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Granska Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav för Azure-informationsskydd](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Ladda ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
