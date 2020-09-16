---
title: Skapa en webbplats i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732260"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="7730b-102">Skapa SharePoint-webbplatser med hjälp av mallar</span><span class="sxs-lookup"><span data-stu-id="7730b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="7730b-103">Det går inte att spara en webbplats som en mall med moderna kommunikations-och grupp webbplatser.</span><span class="sxs-lookup"><span data-stu-id="7730b-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="7730b-104">Mer information om hur du använder mallar finns i [Spara, ladda ned och överföra en SharePoint-webbplats som en mall](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="7730b-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="7730b-105">Här är några vanliga problem/lösningar för att spara en webbplats eller lista som en mall i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7730b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="7730b-106">**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**</span><span class="sxs-lookup"><span data-stu-id="7730b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="7730b-107">Administratörer måste tillåta anpassade skript för att aktivera funktionerna.</span><span class="sxs-lookup"><span data-stu-id="7730b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="7730b-108">Detaljerade anvisningar finns i exempel och överväganden</span><span class="sxs-lookup"><span data-stu-id="7730b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="7730b-109">Tillåta eller förhindra anpassat skript</span><span class="sxs-lookup"><span data-stu-id="7730b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="7730b-110">Kommandot Spara webbplatsen som mall stöds inte och kan orsaka problem på webbplatser som använder infrastrukturen för SharePoint Server-publicering.</span><span class="sxs-lookup"><span data-stu-id="7730b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="7730b-111">**Det går inte att skapa webbplats mal len eller så fungerar den inte korrekt**</span><span class="sxs-lookup"><span data-stu-id="7730b-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="7730b-112">Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) som inte aktive ras.</span><span class="sxs-lookup"><span data-stu-id="7730b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="7730b-113">Om funktionen inte är tillgänglig för aktivering i den aktuella webbplats samlingen kan du inte använda webbplats mal len för att skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="7730b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="7730b-114">Kontrol lera om det finns listor eller bibliotek som överskrider [begränsningen för listvyn](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan förhindra att en webbplatsmall skapas.</span><span class="sxs-lookup"><span data-stu-id="7730b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="7730b-115">Webbplatsen kanske använder för många resurser och webbplats mal len överskrider gränsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="7730b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="7730b-116">Det är problem att visa data från en lista som använder en uppslags kolumn.</span><span class="sxs-lookup"><span data-stu-id="7730b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="7730b-117">Mer information finns i [den här listan visar inte data från rätt uppslags lista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="7730b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="7730b-118">Mer detaljerad information om vanliga problem och lösningar finns i [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="7730b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



