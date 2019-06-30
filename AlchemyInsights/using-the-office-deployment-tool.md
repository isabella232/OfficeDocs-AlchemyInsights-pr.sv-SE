---
title: Med hjälp av verktyget Office Deployment
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365543"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="efdd7-102">Med hjälp av Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="efdd7-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="efdd7-103">Du kan använda Office Deployment Tool (ODT) för att distribuera Office 365-versioner av Office.</span><span class="sxs-lookup"><span data-stu-id="efdd7-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="efdd7-104">Office Deployment Tool (setup.exe) körs från kommandoraden och använder en XML-konfigurationsfil för att avgöra vilka inställningar som ska gälla när du distribuerar Office.</span><span class="sxs-lookup"><span data-stu-id="efdd7-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="efdd7-105">Hämta den senaste versionen av Office Deployment Tool på [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="efdd7-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="efdd7-106">Använd [Verktyget Office-anpassning (ULT)](https://config.office.com) för att välja inställningar för distribution och skapa XML-konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="efdd7-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="efdd7-107">Exportera konfigurationsfilen och placera den i samma mapp som setup.exe finns lokalt.</span><span class="sxs-lookup"><span data-stu-id="efdd7-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="efdd7-108">**Observera:** Office-installationen som ofta uppstår problem förfaller till felkonfigurerad eller konfigurationsfiler för malformatted.</span><span class="sxs-lookup"><span data-stu-id="efdd7-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="efdd7-109">För att undvika sådana problem, rekommenderar vi att du använder verktyget Office-anpassning för att skapa konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="efdd7-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="efdd7-110">Du kan också importera befintliga konfigurationsfiler till verktyget Office-anpassning.</span><span class="sxs-lookup"><span data-stu-id="efdd7-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="efdd7-111">Växla till den plats där setup.exe finns från en kommandotolk och kör verktyget Office Deployment i download-läge och ange den konfigurationsfil som du just har sparat.</span><span class="sxs-lookup"><span data-stu-id="efdd7-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="efdd7-112">I det här exemplet heter konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="efdd7-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="efdd7-113">Kör verktyget Office Deployment i Konfigurera läge och ange konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="efdd7-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="efdd7-114">**Observera:** Du måste köra det här steget från klientdatorn som du vill installera Office och du måste ha lokal administratörsbehörighet på datorn.</span><span class="sxs-lookup"><span data-stu-id="efdd7-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="efdd7-115">Se [Översikt över Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)om du vill veta mer om hur du använder Office Deployment Tool för dina Office 365 ProPlus distributionsscenarier.</span><span class="sxs-lookup"><span data-stu-id="efdd7-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="efdd7-116">Mer information om hur du använder verktyget Office-anpassning finns i [Översikt över verktyget Office-anpassning](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="efdd7-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
