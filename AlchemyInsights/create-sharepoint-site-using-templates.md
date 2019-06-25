---
title: Skapa en webbplats i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199291"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="6e3c8-102">Skapa SharePoint-webbplatser med hjälp av mallar</span><span class="sxs-lookup"><span data-stu-id="6e3c8-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="6e3c8-103">Mallar för SharePoint-webbplatser finns fördefinierade definitioner uppbyggd runt specifika behov.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="6e3c8-104">Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="6e3c8-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="6e3c8-105">Här är några vanliga problem/lösningar om du sparar en webbplats eller lista som en mall i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="6e3c8-106">**Spara platslista/mall-knappen är inte tillgänglig eller saknas**</span><span class="sxs-lookup"><span data-stu-id="6e3c8-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="6e3c8-107">Administratörer måste tillåta anpassat skript ska aktivera Mallfunktioner.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="6e3c8-108">Detaljerade anvisningar finns exempel och överväganden</span><span class="sxs-lookup"><span data-stu-id="6e3c8-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="6e3c8-109">Tillåta eller förhindra att anpassade skript</span><span class="sxs-lookup"><span data-stu-id="6e3c8-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="6e3c8-110">Spara webbplats som mall-kommando stöds inte och kan orsaka problem på platser som använder SharePoint Server Publishing infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="6e3c8-111">**Mallen kan inte skapas eller fungerar inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="6e3c8-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="6e3c8-112">Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktivera inte.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="6e3c8-113">Om funktionen inte är tillgänglig i den aktuella webbplatssamlingen aktivera kan du inte använda mallen för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="6e3c8-114">Kontrollera om eventuella listor eller bibliotek överskrider [Listvyns tröskel som gränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklar som detta kan blockera skapandet av en webbplatsmall.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="6e3c8-115">Webbplatsen kanske använder för många resurser och därför webbplatsmallen överskrider gränsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="6e3c8-116">Det finns problem med visning av data från en lista som använder en uppslagskolumn.</span><span class="sxs-lookup"><span data-stu-id="6e3c8-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="6e3c8-117">Mer information finns i [listan mall skapas inte visar data från rätt söklistan i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="6e3c8-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="6e3c8-118">Mer detaljerad information om vanliga problem och lösningar finns i [Skapa och använda mallar för webbplatser](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="6e3c8-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



