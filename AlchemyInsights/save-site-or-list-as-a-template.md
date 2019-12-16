---
title: Spara webbplats eller lista som en mall
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048742"
---
# <a name="save-site-or-list-as-a-template"></a>Spara webbplats eller lista som en mall

SharePoint-webbplatsmallar är fördefinierade definitioner som utformats kring ett visst affärsbehov. Mer information finns [i använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Här är några vanliga problem/lösningar när du sparar en webbplats eller lista som en mall i SharePoint Online.

**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**. 

- Administratörer måste tillåta anpassade skript för att aktivera mallfunktionerna. Detaljerade anvisningar, exempel och överväganden finns i [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing-infrastrukturen.


**Det går inte att skapa webbplatsmallen eller fungerar inte korrekt**

- Mallen kan sakna en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och kommer inte att aktiveras. Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.


- Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [Listvygränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.


- Webbplatsen kan använda för många resurser och därför webbplatsmallen överskrider gränsen 50 megabyte (MB).


- Det finns problem med att visa data från en lista som använder en uppslagskolumn. Mer information finns [i mallgenererade listan visas inte data från rätt uppslagslistan i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


För mer detaljerad information om vanliga problem och lösningar hänvisas till, [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

