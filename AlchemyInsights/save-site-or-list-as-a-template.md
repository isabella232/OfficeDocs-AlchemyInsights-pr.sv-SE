---
title: Spara webbplats eller lista som en mall
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727549"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="75eef-102">Spara webbplats eller lista som en mall</span><span class="sxs-lookup"><span data-stu-id="75eef-102">Save site or list as a template</span></span>

<span data-ttu-id="75eef-103">SharePoint-webbplatsmallar är färdiga definitioner som utformats kring ett specifikt företags behov.</span><span class="sxs-lookup"><span data-stu-id="75eef-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="75eef-104">Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="75eef-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="75eef-105">Här är några vanliga problem/lösningar för att spara en webbplats eller lista som en mall i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="75eef-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="75eef-106">**Knappen Spara webbplats-listmall är inte tillgänglig eller saknas**.</span><span class="sxs-lookup"><span data-stu-id="75eef-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="75eef-107">Administratörer måste tillåta anpassade skript för att aktivera funktionerna.</span><span class="sxs-lookup"><span data-stu-id="75eef-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="75eef-108">Detaljerade anvisningar finns i exempel och överväganden i [tillåta eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="75eef-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="75eef-109">Kommandot Spara webbplatsen som mall stöds inte och kan orsaka problem på webbplatser som använder infrastrukturen för SharePoint Server-publicering.</span><span class="sxs-lookup"><span data-stu-id="75eef-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="75eef-110">**Det går inte att skapa webbplats mal len eller så fungerar den inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="75eef-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="75eef-111">Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) som inte aktive ras.</span><span class="sxs-lookup"><span data-stu-id="75eef-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="75eef-112">Om funktionen inte är tillgänglig för aktivering i den aktuella webbplats samlingen kan du inte använda webbplats mal len för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="75eef-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="75eef-113">Kontrol lera om det finns listor eller bibliotek som överskrider [begränsningen för listvyn](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan förhindra att en webbplatsmall skapas.</span><span class="sxs-lookup"><span data-stu-id="75eef-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="75eef-114">Webbplatsen kanske använder för många resurser och webbplats mal len överskrider gränsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="75eef-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="75eef-115">Det är problem att visa data från en lista som använder en uppslags kolumn.</span><span class="sxs-lookup"><span data-stu-id="75eef-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="75eef-116">Mer information finns i [den här listan visar inte data från rätt uppslags lista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="75eef-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="75eef-117">Mer detaljerad information om vanliga problem och lösningar finns i [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="75eef-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

