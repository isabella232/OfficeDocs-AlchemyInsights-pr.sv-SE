---
title: Spara webbplats eller lista som en mall
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243745"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="28b1a-102">Spara webbplats eller lista som en mall</span><span class="sxs-lookup"><span data-stu-id="28b1a-102">Save site or list as a template</span></span>

<span data-ttu-id="28b1a-103">Mallar för SharePoint-webbplatser finns fördefinierade definitioner uppbyggd runt specifika behov.</span><span class="sxs-lookup"><span data-stu-id="28b1a-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="28b1a-104">Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="28b1a-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="28b1a-105">Här är några vanliga problem/lösningar om du sparar en webbplats eller lista som en mall i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="28b1a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="28b1a-106">**Spara plats/list knappen mall är inte tillgänglig eller saknas**.</span><span class="sxs-lookup"><span data-stu-id="28b1a-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="28b1a-107">Administratörer måste tillåta anpassat skript ska aktivera Mallfunktioner.</span><span class="sxs-lookup"><span data-stu-id="28b1a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="28b1a-108">Detaljerade anvisningar, exempel och överväganden finns [Tillåt eller förhindra att skriptet](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="28b1a-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="28b1a-109">Spara webbplats som mall-kommando stöds inte och kan orsaka problem på platser som använder SharePoint Server Publishing infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="28b1a-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="28b1a-110">**Mallen kan inte skapas eller fungerar inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="28b1a-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="28b1a-111">Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktivera inte.</span><span class="sxs-lookup"><span data-stu-id="28b1a-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="28b1a-112">Om funktionen inte är tillgänglig i den aktuella webbplatssamlingen aktivera kan du inte använda mallen för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="28b1a-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="28b1a-113">Kontrollera om eventuella listor eller bibliotek överskrider [Listvyns tröskel som gränsen](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklar som detta kan blockera skapandet av en webbplatsmall.</span><span class="sxs-lookup"><span data-stu-id="28b1a-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="28b1a-114">Webbplatsen kanske använder för många resurser och därför webbplatsmallen överskrider gränsen 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="28b1a-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="28b1a-115">Det finns problem med visning av data från en lista som använder en uppslagskolumn.</span><span class="sxs-lookup"><span data-stu-id="28b1a-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="28b1a-116">Mer information finns i [listan mall skapas inte visar data från rätt söklistan i SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="28b1a-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="28b1a-117">Ange referens, [Skapa och använda mallar](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)för mer detaljerad information om vanliga problem och lösningar.</span><span class="sxs-lookup"><span data-stu-id="28b1a-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

