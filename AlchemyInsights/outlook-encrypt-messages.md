---
title: S/MIME i Outlook på webben
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764890"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptera e-postmeddelanden i Outlook

Microsoft 365 Message Encryption bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure Information Protection. Om din prenumeration innehåller Azure Rights Management eller Azure Information Protection **behöver du inte vidta några åtgärder för att manuellt aktivera eller aktivera** Rights Management Service.

Baserat på feedback från kunder kommer vi inte längre att aktivera Exchange-regler för e-postflöde för att automatiskt kryptera utgående e-post som innehåller viss typ av känslig information i din klientorganisation som standard. I stället ger vi detaljerade instruktioner om hur ni själva kan göra det. Mer information om hur du skapar en transportregel för att kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).

- Om du använder Outlook på webben (tidigare **OWA**): När du skriver ett e-postmeddelande klickar du bara på **Skydda** i OWA. Detta gäller behörigheten "Vidarebefordra inte". Klicka på **Ändra behörighet** och välj **Kryptera** om du bara vill kryptera meddelandet.

- Om du använder **Outlook-klienten**: Om du vill skicka ett krypterat meddelande från Outlook 2013 eller 2016 eller Outlook 2016 för Mac väljer du > **Alternativbehörigheter**och väljer sedan det skyddsalternativ du behöver. **Options**

- Om du **vill kryptera alla e-postmeddelanden** som skickas till vissa mottagare eller externa partnerorganisationer automatiskt måste du skapa en transportregel för e-postflöde i Administrationscenter för Exchange. Detaljerade instruktioner finns i [den här supportartikeln](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

