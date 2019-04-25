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
# <a name="save-site-or-list-as-a-template"></a>Spara webbplats eller lista som en mall

Mallar för SharePoint-webbplatser finns fördefinierade definitioner uppbyggd runt specifika behov. Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Här är några vanliga problem/lösningar om du sparar en webbplats eller lista som en mall i SharePoint Online.

**Spara plats/list knappen mall är inte tillgänglig eller saknas**. 

- Administratörer måste tillåta anpassat skript ska aktivera Mallfunktioner. Detaljerade anvisningar, exempel och överväganden finns [Tillåt eller förhindra att skriptet](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


- Spara webbplats som mall-kommando stöds inte och kan orsaka problem på platser som använder SharePoint Server Publishing infrastruktur.


**Mallen kan inte skapas eller fungerar inte korrekt**

- Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktivera inte. Om funktionen inte är tillgänglig i den aktuella webbplatssamlingen aktivera kan du inte använda mallen för att skapa en webbplats.


- Kontrollera om eventuella listor eller bibliotek överskrider [Listvyns tröskel som gränsen](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklar som detta kan blockera skapandet av en webbplatsmall.


- Webbplatsen kanske använder för många resurser och därför webbplatsmallen överskrider gränsen 50 megabyte (MB).


- Det finns problem med visning av data från en lista som använder en uppslagskolumn. Mer information finns i [listan mall skapas inte visar data från rätt söklistan i SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Ange referens, [Skapa och använda mallar](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)för mer detaljerad information om vanliga problem och lösningar.

