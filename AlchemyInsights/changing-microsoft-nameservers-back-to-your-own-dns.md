---
title: Ändra från Microsofts namnservrar tillbaka till att hantera dina egna DNS-poster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506974"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Ändra från Microsofts namnservrar tillbaka till att hantera dina egna DNS-poster

Du har tidigare ändrat NS-posterna så att de pekar på Microsoft (ns1.bdm.microsoftonline.com) men har nu bestämt dig för att hantera dina egna DNS-poster:

Ändra namnservern tillbaka till registratorn eller den tidigare inställningen på din domänregistrators webbplats. Om du inte är bekant med DNS kontaktar du supporten hos domänregistratorn. Observera att det kan ta upp till 48 timmar innan namnserverändringar har spridits. 

1. I Microsoft 365-administratörsportalen **går du till Inställningar** Domäner , markerar kryssrutan bredvid domänen och väljer Hantera  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **DNS.** 

2. I guiden väljer du Lägg **till dina egna DNS-poster** och slutför guiden. Detta ändrar hur din DNS hanteras och gör att du kan lägga till de anpassade DNS-poster som behövs för att stödja dina valda tjänster.

Om du har ändrat namnserverposterna till Microsoft och har en webbplats kan du lägga till DNS-poster för webbplatsen i stället för att ändra namnservrarna igen. Mer information finns i Uppdatera [DNS-poster för att behålla webbplatsen hos ditt nuvarande webbhotell.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


