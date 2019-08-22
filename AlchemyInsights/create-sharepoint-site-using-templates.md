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
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515016"
---
# <a name="create-sharepoint-sites-using-templates"></a>Skapa SharePoint-webbplatser med hjälp av mallar

Mallar för SharePoint-webbplatser finns fördefinierade definitioner uppbyggd runt specifika behov. Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Här är några vanliga problem/lösningar om du sparar en webbplats eller lista som en mall i Sharepoint Online. 

**Spara platslista/mall-knappen är inte tillgänglig eller saknas**

Administratörer måste tillåta anpassat skript ska aktivera Mallfunktioner. Detaljerade anvisningar finns exempel och överväganden 

- [Tillåta eller förhindra att anpassade skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Spara webbplats som mall-kommando stöds inte och kan orsaka problem på platser som använder SharePoint Server Publishing infrastruktur.

**Mallen kan inte skapas eller fungerar inte korrekt**

Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktivera inte. Om funktionen inte är tillgänglig i den aktuella webbplatssamlingen aktivera kan du inte använda mallen för att skapa en webbplats.

- Kontrollera om eventuella listor eller bibliotek överskrider [Listvyns tröskel som gränsen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklar som detta kan blockera skapandet av en webbplatsmall.

- Webbplatsen kanske använder för många resurser och därför webbplatsmallen överskrider gränsen på 50 MB.


- Det finns problem med visning av data från en lista som använder en uppslagskolumn. Mer information finns i [listan mall skapas inte visar data från rätt söklistan i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Mer detaljerad information om vanliga problem och lösningar finns i [Skapa och använda mallar för webbplatser](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



