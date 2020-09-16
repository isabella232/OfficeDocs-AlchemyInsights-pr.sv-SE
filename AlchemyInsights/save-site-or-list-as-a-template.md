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
# <a name="save-site-or-list-as-a-template"></a>Spara webbplats eller lista som en mall

SharePoint-webbplatsmallar är färdiga definitioner som utformats kring ett specifikt företags behov. Mer information finns i [använda mallar för att skapa olika typer av SharePoint-webbplatser](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Här är några vanliga problem/lösningar för att spara en webbplats eller lista som en mall i SharePoint Online.

**Knappen Spara webbplats-listmall är inte tillgänglig eller saknas**. 

- Administratörer måste tillåta anpassade skript för att aktivera funktionerna. Detaljerade anvisningar finns i exempel och överväganden i [tillåta eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Kommandot Spara webbplatsen som mall stöds inte och kan orsaka problem på webbplatser som använder infrastrukturen för SharePoint Server-publicering.


**Det går inte att skapa webbplats mal len eller så fungerar den inte korrekt**

- Mallen saknar en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) som inte aktive ras. Om funktionen inte är tillgänglig för aktivering i den aktuella webbplats samlingen kan du inte använda webbplats mal len för att skapa en webbplats.


- Kontrol lera om det finns listor eller bibliotek som överskrider [begränsningen för listvyn](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) för 5000 objekt eftersom detta kan förhindra att en webbplatsmall skapas.


- Webbplatsen kanske använder för många resurser och webbplats mal len överskrider gränsen på 50 MB.


- Det är problem att visa data från en lista som använder en uppslags kolumn. Mer information finns i [den här listan visar inte data från rätt uppslags lista i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Mer detaljerad information om vanliga problem och lösningar finns i [skapa och använda webbplatsmallar](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

