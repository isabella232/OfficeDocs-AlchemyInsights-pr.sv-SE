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
# <a name="create-sharepoint-sites-using-templates"></a>Skapa SharePoint-webbplatser med hjälp av mallar

Möjligheten att spara en webbplats som mall stöds inte med moderna kommunikations- eller teamwebbplatser. Mer information om hur du använder mallar finns i [Spara, hämta och överföra en SharePoint-webbplats som en mall](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Här är några vanliga problem/lösningar om att spara en webbplats eller lista som en mall i Sharepoint Online. 

**Knappen Spara webbplats/lista mall är inte tillgänglig eller saknas**

Administratörer måste tillåta anpassat skript för att aktivera mallfunktionerna. Detaljerade steg finns i 

- [Tillåta eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandot Spara webbplats som mall stöds inte och kan orsaka problem på webbplatser som använder SharePoint Server Publishing Infrastructure.

**Webbplatsmallen kan inte skapas eller fungerar inte korrekt**

Mallen kanske saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) och aktiveras inte. Om funktionen inte är tillgänglig för aktivering i den aktuella webbplatssamlingen kan du inte använda webbplatsmallen för att skapa en webbplats.

- Kontrollera om några listor eller bibliotek överskrider tröskelvärdet för [listvygräns](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan blockera skapandet av en webbplatsmall.

- Webbplatsen kan använda för många resurser och därför överskrider webbplatsmallen 50 MB gränsen.


- Det finns problem med att visa data från en lista som använder en uppslagskolumn. Mer information finns i [Mallgenererad lista visar inte data från rätt uppslagslista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Mer detaljerad information om vanliga problem och lösningar finns i [Skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



