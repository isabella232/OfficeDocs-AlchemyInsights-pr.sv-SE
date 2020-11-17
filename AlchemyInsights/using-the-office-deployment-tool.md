---
title: Använda distributions verktyget för Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085850"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="f7aab-102">Använda distributions verktyget för Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="f7aab-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f7aab-103">Du använder Office Deployment Tool (ODT) för att distribuera Office 365-versioner av Office.</span><span class="sxs-lookup"><span data-stu-id="f7aab-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="f7aab-104">Distributions verktyget för Office (setupodt.exe) körs från kommando raden och använder en XML-konfigurationsfil för att bestämma vilka inställningar som ska användas vid distribution av Office.</span><span class="sxs-lookup"><span data-stu-id="f7aab-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="f7aab-105">Ladda ner den senaste versionen av distributions verktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f7aab-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="f7aab-106">Använd [verktyget för anpassning av Office (ULT)](https://config.office.com) för att välja distributions inställningar och skapa XML-konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="f7aab-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="f7aab-107">Exportera konfigurations filen och placera den lokalt på samma mapp där setupodt.exe finns.</span><span class="sxs-lookup"><span data-stu-id="f7aab-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="f7aab-108">**Obs!** Problem med Office-installationer uppstår ofta på grund av felkonfigurerade eller malformatted.</span><span class="sxs-lookup"><span data-stu-id="f7aab-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="f7aab-109">För att undvika sådana problem rekommenderar vi att du använder verktyget Office-anpassning för att skapa konfigurations filen.</span><span class="sxs-lookup"><span data-stu-id="f7aab-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="f7aab-110">Du kan också importera befintliga konfigurationsfiler till verktyget för Office-anpassning.</span><span class="sxs-lookup"><span data-stu-id="f7aab-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="f7aab-111">Gå till den plats där setupodt.exe finns i en upphöjd kommando tolk och kör distributions verktyget för Office i nedladdnings läge och ange konfigurations filen du just sparade.</span><span class="sxs-lookup"><span data-stu-id="f7aab-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="f7aab-112">I det här exemplet heter konfigurations filen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="f7aab-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="f7aab-113">4. kör distributions verktyget för Office i läget konfiguration och ange konfigurations filen.</span><span class="sxs-lookup"><span data-stu-id="f7aab-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="f7aab-114">**Obs!** Du måste köra det här steget från den klient dator där du vill installera Office och måste ha lokal administratörs behörighet på den datorn.</span><span class="sxs-lookup"><span data-stu-id="f7aab-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="f7aab-115">Mer information om hur du använder distributions verktyget för Microsoft 365 för företags distributions scenarier finns i [Översikt över distributions verktyget för Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="f7aab-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="f7aab-116">Mer information om hur du använder verktyget Office-anpassning finns i [Översikt över verktyget Office-anpassning](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="f7aab-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
