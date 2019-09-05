---
title: Spara webbplats eller lista som en mall
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752050"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="b2b8b-102">Spara webbplats eller lista som en mall</span><span class="sxs-lookup"><span data-stu-id="b2b8b-102">Save site or list as a template</span></span>

<span data-ttu-id="b2b8b-103">SharePoint-webbplatsmallar är fördefinierade definitioner som utformats kring ett visst affärsbehov.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="b2b8b-104">Mer information finns [i använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="b2b8b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="b2b8b-105">Här är några vanliga problem/lösningar när du sparar en webbplats eller lista som en mall i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="b2b8b-106">**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="b2b8b-107">Administratörer måste tillåta anpassade skript för att aktivera mallfunktionerna.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="b2b8b-108">Detaljerade anvisningar, exempel och överväganden finns i [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b2b8b-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="b2b8b-109">Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing-infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="b2b8b-110">**Det går inte att skapa webbplatsmallen eller fungerar inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="b2b8b-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="b2b8b-111">Mallen kan sakna en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och kommer inte att aktiveras.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="b2b8b-112">Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="b2b8b-113">Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [Listvygränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="b2b8b-114">Webbplatsen kan använda för många resurser och därför webbplatsmallen överskrider gränsen 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="b2b8b-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="b2b8b-115">Det finns problem med att visa data från en lista som använder en uppslagskolumn.</span><span class="sxs-lookup"><span data-stu-id="b2b8b-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="b2b8b-116">Mer information finns [i mallgenererade listan visas inte data från rätt uppslagslistan i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="b2b8b-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="b2b8b-117">För mer detaljerad information om vanliga problem och lösningar hänvisas till, [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="b2b8b-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

