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
# <a name="create-sharepoint-sites-using-templates"></a>Skapa SharePoint-webbplatser med hjälp av mallar

Det går inte att spara en webbplats som en mall med moderna kommunikations-och grupp webbplatser. Mer information om hur du använder mallar finns i [Spara, ladda ned och överföra en SharePoint-webbplats som en mall](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Här är några vanliga problem/lösningar för att spara en webbplats eller lista som en mall i SharePoint Online. 

**Knappen Spara webbplats/listmall är inte tillgänglig eller saknas**

Administratörer måste tillåta anpassade skript för att aktivera funktionerna. Detaljerade anvisningar finns i exempel och överväganden 

- [Tillåta eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandot Spara webbplatsen som mall stöds inte och kan orsaka problem på webbplatser som använder infrastrukturen för SharePoint Server-publicering.

**Det går inte att skapa webbplats mal len eller så fungerar den inte korrekt**

Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) som inte aktive ras. Om funktionen inte är tillgänglig för aktivering i den aktuella webbplats samlingen kan du inte använda webbplats mal len för att skapa en webbplats.

- Kontrol lera om det finns listor eller bibliotek som överskrider [begränsningen för listvyn](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan förhindra att en webbplatsmall skapas.

- Webbplatsen kanske använder för många resurser och webbplats mal len överskrider gränsen på 50 MB.


- Det är problem att visa data från en lista som använder en uppslags kolumn. Mer information finns i [den här listan visar inte data från rätt uppslags lista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Mer detaljerad information om vanliga problem och lösningar finns i [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



