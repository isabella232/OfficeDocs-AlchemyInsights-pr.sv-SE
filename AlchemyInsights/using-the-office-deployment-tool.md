---
title: Med hjälp av verktyget Office Deployment
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492097"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="2f27c-102">Med hjälp av Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="2f27c-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="2f27c-p101">Du kan använda Office Deployment Tool (ODT) för att distribuera Office 365-versioner av Office. Office Deployment Tool (setup.exe) körs från kommandoraden och använder en XML-konfigurationsfil för att avgöra vilka inställningar som ska gälla när du distribuerar Office.</span><span class="sxs-lookup"><span data-stu-id="2f27c-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="2f27c-105">Hämta den senaste versionen av Office Deployment Tool på [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="2f27c-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="2f27c-p102">Använd [Verktyget Office-anpassning (ULT)](https://config.office.com) för att välja inställningar för distribution och skapa XML-konfigurationsfilen. Exportera konfigurationsfilen och placera den i samma mapp som setup.exe finns lokalt.</span><span class="sxs-lookup"><span data-stu-id="2f27c-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="2f27c-p103">**Observera:** Office-installationen som ofta uppstår problem förfaller till felkonfigurerad eller konfigurationsfiler för malformatted. För att undvika sådana problem, rekommenderar vi att du använder verktyget Office-anpassning för att skapa konfigurationsfilen. Du kan också importera befintliga konfigurationsfiler till verktyget Office-anpassning.</span><span class="sxs-lookup"><span data-stu-id="2f27c-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="2f27c-p104">Växla till den plats där setup.exe finns från en kommandotolk och kör verktyget Office Deployment i download-läge och ange den konfigurationsfil som du just har sparat. I det här exemplet heter konfigurationsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="2f27c-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="2f27c-113">Kör verktyget Office Deployment i Konfigurera läge och ange konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="2f27c-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="2f27c-114">**Observera:** Du måste köra det här steget från klientdatorn som du vill installera Office och du måste ha lokal administratörsbehörighet på datorn.</span><span class="sxs-lookup"><span data-stu-id="2f27c-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="2f27c-p105">Se [Översikt över Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)om du vill veta mer om hur du använder Office Deployment Tool för dina Office 365 ProPlus distributionsscenarier. Mer information om hur du använder verktyget Office-anpassning finns i [Översikt över verktyget Office-anpassning](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="2f27c-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

