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
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794850"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Hantera organisationens globala adresslista och offlineadressbok

En global adresslista är en lista över e-postaktiverade objekt (alla typer av mottagare som kan ta emot e-post) i organisationen. En global adresslista skapas automatiskt i alla organisationer. Du kan skapa flera globala adresslistor för att separera användare efter organisation eller plats, men en enskild användare kan bara se och använda en global adresslista i taget.

Vissa e-postklienter, till exempel Outlook för Windows, laddar ned den globala adresslistan för offlineanvändning. Det kallas offlineadressbok. Exchange Online uppdateras en offlineadressbok bara en gång var 8:e timme och sedan måste klienterna ladda ned den för att uppdatera den lokala kopian av offlineadressboken. Alla mottagarändringar måste först synas i den globala adresslistan för att senare hamna i offlineadressboken.

Här är några vanliga procedurer för global adresslista och offlineadressbok:

- Av olika anledningar kanske du vill dölja vissa objekt i den globala adresslistan. Se [Dölja mottagare i adresslistor](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Om du behöver ge specifika grupper anpassade vyer av organisationens globala adresslista kan du läsa artikeln om [adressboksprinciper i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Skapa en global adresslista i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) och om du vill lära dig hur du arbetar med behörigheter för globala adresslistor läser du artikeln om [adresslistor i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Obs! Om du vill skapa nya globala adresslistor kanske du även vill skapa en ny offlineadressbok. Se artikeln om [procedurer för offlineadressböcker](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
