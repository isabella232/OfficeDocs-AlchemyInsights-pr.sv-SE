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
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770441"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="f53cd-102">Skapa SharePoint-webbplatser med hjälp av mallar</span><span class="sxs-lookup"><span data-stu-id="f53cd-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="f53cd-103">Möjligheten att spara en webbplats som mall stöds inte med moderna kommunikations- eller teamwebbplatser.</span><span class="sxs-lookup"><span data-stu-id="f53cd-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="f53cd-104">Mer information om hur du använder mallar finns i [Spara, hämta och överföra en SharePoint-webbplats som en mall](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="f53cd-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="f53cd-105">Här är några vanliga problem/lösningar om att spara en webbplats eller lista som en mall i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="f53cd-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="f53cd-106">**Knappen Spara webbplats/lista mall är inte tillgänglig eller saknas**</span><span class="sxs-lookup"><span data-stu-id="f53cd-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="f53cd-107">Administratörer måste tillåta anpassat skript för att aktivera mallfunktionerna.</span><span class="sxs-lookup"><span data-stu-id="f53cd-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f53cd-108">Detaljerade steg finns i</span><span class="sxs-lookup"><span data-stu-id="f53cd-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="f53cd-109">Tillåta eller förhindra anpassat skript</span><span class="sxs-lookup"><span data-stu-id="f53cd-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="f53cd-110">Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing Infrastructure.</span><span class="sxs-lookup"><span data-stu-id="f53cd-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="f53cd-111">**Webbplatsmallen kan inte skapas eller fungerar inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="f53cd-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="f53cd-112">Mallen kanske saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktiveras inte.</span><span class="sxs-lookup"><span data-stu-id="f53cd-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="f53cd-113">Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="f53cd-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="f53cd-114">Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [listvygräns](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.</span><span class="sxs-lookup"><span data-stu-id="f53cd-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="f53cd-115">Webbplatsen kan använda för många resurser och därför överskrider webbplatsmallen 50 MB gränsen.</span><span class="sxs-lookup"><span data-stu-id="f53cd-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="f53cd-116">Det finns problem med att visa data från en lista som använder en uppslagskolumn.</span><span class="sxs-lookup"><span data-stu-id="f53cd-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f53cd-117">Mer information finns i [Mallgenererad lista visar inte data från rätt uppslagslista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="f53cd-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="f53cd-118">Mer detaljerad information om vanliga problem och lösningar finns i [Skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="f53cd-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



