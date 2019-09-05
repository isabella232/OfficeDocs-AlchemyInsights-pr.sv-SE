---
title: Skapa en webbplats i SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755326"
---
# <a name="create-sharepoint-sites-using-templates"></a>Skapa SharePoint-webbplatser med hjälp av mallar

SharePoint-webbplatsmallar är fördefinierade definitioner som utformats kring ett visst affärsbehov. Mer information finns [i använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Här är några vanliga problem/lösningar när du sparar en webbplats eller lista som en mall i SharePoint Online. 

**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**

Administratörer måste tillåta anpassade skript för att aktivera mallfunktionerna. För detaljerade steg, exempel och överväganden, se 

- [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing-infrastrukturen.

**Det går inte att skapa webbplatsmallen eller fungerar inte korrekt**

Mallen kan sakna en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och kommer inte att aktiveras. Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.

- Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [Listvygränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.

- Webbplatsen kan använda för många resurser och därför överskrider webbplatsmallen gränsen på 50 MB.


- Det finns problem med att visa data från en lista som använder en uppslagskolumn. Mer information finns [i mallgenererade listan visas inte data från rätt uppslagslistan i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

För mer detaljerad information om vanliga problem och lösningar, vänligen kontrollera [skapa och Använd webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



