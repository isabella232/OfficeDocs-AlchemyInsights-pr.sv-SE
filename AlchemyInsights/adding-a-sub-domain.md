---
title: Lägga till en underdomän
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506769"
---
# <a name="adding-a-sub-domain"></a>Lägga till en underdomän

Underdomäner kan läggas till i samma eller en annan klientorganisation än den överordnade domänen. I båda fallen måste du hantera dina egna DNS-inställningar på registratorns webbplats. Om du låter Microsoft hantera dina DNS-inställningar med NS-poster, eller om du har köpt domänen från Microsoft, kan du inte lägga till underdomäner utan att ändra detta först.

Lägg först till den överordnade domänen och sedan lägga till underdomänen. Om underdomänen finns i samma klientorganisation krävs ingen ytterligare verifiering. Om du lägger till underdomänen i en separat klientorganisation krävs DNS txt-posten för ägarbekräftelse innan du lägger till domänen och de ytterligare DNS-posterna för de valda tjänsterna.

- Om du vill lägga till en domän eller underdomän följer du guiden Lägg till domän [eller](https://admin.microsoft.com/Adminportal#/Domains/Wizard)lägger till domänen eller underdomänen manuellt genom att gå till **Ange** domäner Lägg  >    >  **till domän.**

Om det behövs:

- Om du vill ändra vem som hanterar dina DNS-inställningar för en befintlig domän går du till **Inställningar** Domains , markerar kryssrutan bredvid domänen och väljer  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)sedan **Manage DNS.** I guiden väljer du Lägg **till dina egna DNS-poster** och slutför guiden.
- Om du vill lägga till underdomäner i en domän som köpts av Microsoft överför du först domänen till en annan registrator och gör sedan ändringen ovan för att hantera dina egna DNS-poster. Anvisningar finns i Överföra [en domän från Microsoft till en annan värd.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Om du får ett felmeddelande om att domänen redan används av andra medlemmar eller personer i organisationen måste du först ta över det här ohanterade kontot innan du använder domänen. Instruktioner finns i [Ta över en ohanterad katalog som administratör i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
