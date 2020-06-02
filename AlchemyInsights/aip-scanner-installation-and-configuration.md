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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="81c94-102">AIP-skanner: installation och konfiguration</span><span class="sxs-lookup"><span data-stu-id="81c94-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="81c94-103">**Så här installerar du AIP-skannern:**</span><span class="sxs-lookup"><span data-stu-id="81c94-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="81c94-104">Om du uppgraderar och inte utför en ren installation, se till att du har följt riktlinjerna för [uppgradering av Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) och för enhetlig märkning klient, se uppgradera Azure Information Protection [scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="81c94-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="81c94-105">Kontrollera att du uppfyller alla krav på [brandväggar och inställningar för nätverksinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="81c94-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="81c94-106">Kontrollera att dina [principer är inställda på](https://docs.microsoft.com/azure/information-protection/configure-policy) automatisk märkning eller har en standardetikett i principen.</span><span class="sxs-lookup"><span data-stu-id="81c94-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="81c94-107">Kontrollera att den relevanta filtypen är konfigurerad för etikett/skydd enligt beskrivningen i Filtyper som [stöds av Azure Information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="81c94-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="81c94-108">Om du vill ändra standardbeteendet följer du dessutom dessa riktlinjer: [Ändra standardskyddsnivån för filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="81c94-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="81c94-109">Kontrollera att användarkontot som konfigurerats för att köra skannertjänsten har behörighet att komma åt alla konfigurerade databaser.</span><span class="sxs-lookup"><span data-stu-id="81c94-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="81c94-110">Om du fortfarande har problem kan du exportera skannerloggarna och lägga till dem i supportbiljetten.</span><span class="sxs-lookup"><span data-stu-id="81c94-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="81c94-111">**Exportera Azure Information Protection Scanner-loggar**</span><span class="sxs-lookup"><span data-stu-id="81c94-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="81c94-112">Navigera till %localappdata%\Microsoft\MSIP under användarkontexten som kör skannertjänsten.</span><span class="sxs-lookup"><span data-stu-id="81c94-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="81c94-113">Zip allt innehåll under MSIP-mappen.</span><span class="sxs-lookup"><span data-stu-id="81c94-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="81c94-114">Spara loggarna till ditt val av plats och bifoga dem till din servicebegäran.</span><span class="sxs-lookup"><span data-stu-id="81c94-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="81c94-115">Du kan också använda [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="81c94-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="81c94-116">**Mer information finns i:**</span><span class="sxs-lookup"><span data-stu-id="81c94-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="81c94-117">Distribuera Azure Information Protection-skannern för att automatiskt klassificera och skydda filer</span><span class="sxs-lookup"><span data-stu-id="81c94-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="81c94-118">Ange och använda parametern Token för Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="81c94-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="81c94-119">Kör en identifieringscykel och visa rapporter för skannern</span><span class="sxs-lookup"><span data-stu-id="81c94-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="81c94-120">Granska Azure Information Protection-dokumentation</span><span class="sxs-lookup"><span data-stu-id="81c94-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="81c94-121">Krav för Azure-informationsskydd</span><span class="sxs-lookup"><span data-stu-id="81c94-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="81c94-122">Ladda ned Azure Information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="81c94-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)