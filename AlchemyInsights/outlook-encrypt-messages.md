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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010742"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptera e-postmeddelanden i Outlook

Microsoft 365 Meddelandekryptering bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure Information Protection. Om prenumerationen omfattar Azure Rights Management eller Azure Information Protection **behöver** du inte vidta några åtgärder för att manuellt aktivera eller aktivera rättighetshanteringstjänsten.

Baserat på kundfeedback kommer vi inte längre att göra det möjligt för Exchange-postflödesregler att automatiskt kryptera utgående e-postmeddelanden som innehåller viss typ av känslig information i klientorganisationen som standard. I stället ger vi dig detaljerade anvisningar om hur du kan göra det. Mer information om hur du skapar en transportregel för att kryptera känslig information finns i den [här artikeln.](https://aka.ms/OmeEtr)

- Om du Outlook på webben (tidigare **OWA):** När du skriver ett e-postmeddelande klickar du bara **på Skydda** i OWA. Behörigheten Vidarebefordra inte tillämpas. Klicka **på Ändra behörighet** och välj **Kryptera** för att bara kryptera meddelandet.

- Om du använder **Outlook** klient : Om du vill skicka ett krypterat meddelande från Outlook 2013 eller 2016, eller Outlook 2016 för Mac, väljer du Alternativbehörigheter och sedan det skyddsalternativ du  >  behöver.

- Om **du vill att all e-post** som skickas automatiskt ska krypteras till vissa mottagare eller externa partnerorganisationer måste du skapa en transportregel för e-Exchange administrationscentret för e-post. Detaljerade anvisningar finns i den [här supportartikeln.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

