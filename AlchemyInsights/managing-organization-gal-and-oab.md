---
title: Hantera organisationens globala adresslista och offlineadressbok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042180"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Hantera organisationens globala adresslista och offlineadressbok

En global adresslista är en lista över e-postaktiverade objekt (alla typer av mottagare som kan ta emot e-post) i organisationen. En global adresslista skapas automatiskt i alla organisationer. Du kan skapa flera globala adresslistor för att separera användare efter organisation eller plats, men en enskild användare kan bara se och använda en global adresslista i taget.

Vissa e-postklienter, till exempel Outlook för Windows, laddar ned den globala adresslistan för offlineanvändning. Det kallas offlineadressbok. Exchange Online uppdateras en offlineadressbok bara en gång var 8:e timme och sedan måste klienterna ladda ned den för att uppdatera den lokala kopian av offlineadressboken. Alla mottagarändringar måste först synas i den globala adresslistan för att senare hamna i offlineadressboken.

Här är några vanliga procedurer för global adresslista och offlineadressbok:

- Av olika anledningar kanske du vill dölja vissa objekt i den globala adresslistan. Se [Dölja mottagare i adresslistor](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Om du behöver ge specifika grupper anpassade vyer av organisationens globala adresslista kan du läsa artikeln om [adressboksprinciper i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Skapa en global adresslista i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) och om du vill lära dig hur du arbetar med behörigheter för globala adresslistor läser du artikeln om [adresslistor i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Obs! Om du vill skapa nya globala adresslistor kanske du även vill skapa en ny offlineadressbok. Se artikeln om [procedurer för offlineadressböcker](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
