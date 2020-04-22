---
title: Använda distributionsverktyget för Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726266"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="860b2-102">Använda Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="860b2-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="860b2-103">Du kan använda OFFICE Deployment Tool (ODT) för att distribuera Office 365-versioner av Office.</span><span class="sxs-lookup"><span data-stu-id="860b2-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="860b2-104">Office Deployment Tool (setup.exe) körs från kommandoraden och använder en XML-fil för konfiguration för att avgöra vilka inställningar som ska gälla vid distribution av Office.</span><span class="sxs-lookup"><span data-stu-id="860b2-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="860b2-105">Hämta den senaste versionen av Distributionsverktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="860b2-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="860b2-106">Använd [Office Customization Tool (OCT)](https://config.office.com) för att välja distributionsinställningar och skapa konfigurations-XML-filen.</span><span class="sxs-lookup"><span data-stu-id="860b2-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="860b2-107">Exportera konfigurationsfilen och placera den lokalt i samma mapp där setup.exe finns.</span><span class="sxs-lookup"><span data-stu-id="860b2-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="860b2-108">**Anm.:** Problem med Office-installation uppstår ofta på grund av felkonfigurerade eller felformaterade konfigurationsfiler.</span><span class="sxs-lookup"><span data-stu-id="860b2-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="860b2-109">För att undvika sådana problem rekommenderar vi att du använder Anpassningsverktyget för Office för att skapa konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="860b2-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="860b2-110">Du kan också importera befintliga konfigurationsfiler till Anpassningsverktyget för Office.</span><span class="sxs-lookup"><span data-stu-id="860b2-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="860b2-111">Från en upphöjd kommandotolk växlar du till den plats där setup.exe finns och kör Office Deployment Tool i nedladdningsläge och anger konfigurationsfilen som du just sparade.</span><span class="sxs-lookup"><span data-stu-id="860b2-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="860b2-112">I det här exemplet heter konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="860b2-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="860b2-113">Kör Office Deployment Tool i konfigurera läge och ange konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="860b2-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="860b2-114">**Anm.:** Du måste köra det här steget från klientdatorn där du vill installera Office och du måste ha lokala administratörsbehörigheter på den datorn.</span><span class="sxs-lookup"><span data-stu-id="860b2-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="860b2-115">Mer information om hur du använder Distributionsverktyg för Office för microsoft 365-appar för företagsdistributionsscenarier finns [i Översikt över Distributionsverktyget för Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="860b2-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="860b2-116">Mer information om hur du använder Anpassningsverktyget för Office finns i [Översikt över Anpassningsverktyget för Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="860b2-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
