---
title: Skapa en webbplats i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052487"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="60587-102">Skapa SharePoint-webbplatser med hjälp av mallar</span><span class="sxs-lookup"><span data-stu-id="60587-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="60587-103">SharePoint-webbplatsmallar är fördefinierade definitioner som utformats kring ett visst affärsbehov.</span><span class="sxs-lookup"><span data-stu-id="60587-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="60587-104">Mer information finns [i använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="60587-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="60587-105">Här är några vanliga problem/lösningar när du sparar en webbplats eller lista som en mall i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="60587-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="60587-106">**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**</span><span class="sxs-lookup"><span data-stu-id="60587-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="60587-107">Administratörer måste tillåta anpassade skript för att aktivera mallfunktionerna.</span><span class="sxs-lookup"><span data-stu-id="60587-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="60587-108">För detaljerade steg, exempel och överväganden, se</span><span class="sxs-lookup"><span data-stu-id="60587-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="60587-109">Tillåt eller förhindra anpassat skript</span><span class="sxs-lookup"><span data-stu-id="60587-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="60587-110">Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing-infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="60587-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="60587-111">**Det går inte att skapa webbplatsmallen eller fungerar inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="60587-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="60587-112">Mallen kan sakna en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och kommer inte att aktiveras.</span><span class="sxs-lookup"><span data-stu-id="60587-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="60587-113">Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="60587-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="60587-114">Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [Listvygränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.</span><span class="sxs-lookup"><span data-stu-id="60587-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="60587-115">Webbplatsen kan använda för många resurser och därför överskrider webbplatsmallen gränsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="60587-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="60587-116">Det finns problem med att visa data från en lista som använder en uppslagskolumn.</span><span class="sxs-lookup"><span data-stu-id="60587-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="60587-117">Mer information finns [i mallgenererade listan visas inte data från rätt uppslagslistan i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="60587-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="60587-118">För mer detaljerad information om vanliga problem och lösningar, vänligen kontrollera [skapa och Använd webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="60587-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



