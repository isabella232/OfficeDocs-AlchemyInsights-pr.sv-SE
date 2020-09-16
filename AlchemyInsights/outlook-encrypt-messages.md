---
title: S/MIME i Outlook på webben
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772316"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptera e-postmeddelanden i Outlook

Microsoft 365 meddelande kryptering bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure information Protection. Om ditt abonnemang inkluderar Azure Rights Management eller Azure information Protection **behöver du inte vidta några åtgärder för att aktivera eller inaktivera** Rights Management-tjänsten manuellt.

Baserat på feedback från kunder kommer vi inte längre att aktivera regler för Exchange-postflöde för att automatiskt kryptera utgående e-post som innehåller viss typ av känslig information i klient organisationen. I stället tillhandahåller vi detaljerade anvisningar om hur du gör det hör dock. Mer information om hur du skapar en transport regel för att kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).

- Om du använder Outlook på webben (tidigare **OWA**): när du skriver ett e-postmeddelande klickar du helt enkelt på **skydda** i OWA. Detta tillämpar behörigheten "Vidarekoppla inte". Klicka på **Ändra behörighet** och välj **kryptera** för att kryptera meddelandet.

- Om du använder **Outlook-klienten**: för att skicka ett krypterat meddelande från Outlook 2013 eller 2016, eller Outlook 2016 för Mac, väljer du **alternativ**  >  **behörigheter**och väljer sedan det skydds alternativ du behöver.

- För att **automatiskt kryptera alla e-postmeddelanden** som skickas till vissa mottagare eller externa partner organisationer måste du skapa en regel för e-postflödes transport i administrations centret för Exchange. Detaljerade anvisningar finns i [den här Support artikeln](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

