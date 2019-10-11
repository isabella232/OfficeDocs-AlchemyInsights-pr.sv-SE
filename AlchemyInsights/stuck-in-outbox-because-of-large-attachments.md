---
title: Fastnat i Utkorgen på grund av stora bilagor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441323"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Åtgärda meddelanden som har fastnat i Utkorgen

Vi rekommenderar att du börjar med att köra scenariot ["Jag har problem med att skicka, ta emot eller hitta e-postmeddelanden"](https://aka.ms/SaRA-OutlookSendReceive) från verktyget [Microsoft support och återställning assistenten](https://diagnostics.office.com/#/) .

När ett meddelande fastnar i Utkorgen är de mest troliga orsakerna:
- Stora bilagor.
- Alternativet **Skicka omedelbart när anslutet** är inte aktiverat.

Så här tar du bort stora bilagor: 

1. I Outlook väljer du **skicka och ta emot** > **arbete offline**. 
2. Välj **Utkorg**i navigeringsfönstret. Härifrån kan du: 
    - Ta bort meddelandet (Markera det och välj sedan **ta bort**).
    - Dra meddelandet till mappen Utkast, dubbelklicka för att öppna det och ta bort bilagan Markera den och välj sedan **ta bort**).
3. Om du får ett felmeddelande som säger att Outlook försöker skicka meddelandet stänger du Outlook. Det kan ta en stund att avsluta. Om Outlook inte stängs trycker du på Ctrl + Alt + Delete och väljer **Starta Aktivitetshanteraren**. I Aktivitetshanteraren väljer du fliken **processer** , bläddrar ned till Outlook. exe och väljer **Avsluta process**.
4. När Outlook har stängts startar du om det och upprepar steg 2 och 3. 
5. När du tar bort den bifogade filen klickar du på **skicka och ta emot** > **arbete offline** att återuppta arbeta online. 

Meddelanden fastnar också i Utkorgen när du klickar på **Skicka**, men du är inte ansluten. Klicka på **skicka och ta emot** och titta på knappen **arbeta offline** . Om det är blått är du frånkopplad. Välj den för att ansluta (knappen blir vit) och klicka på **skicka alla**.
 
Så här aktiverar du **Skicka omedelbart vid anslutning**:
 
- Välj **fil** > **alternativ** >  **Avancerat**.
I avsnittet **skicka och ta emot** väljer du **Skicka omedelbart när du är ansluten**och väljer sedan **OK**.
 
För fullständig information se:
- [Video: skicka eller ta bort en fast e-post](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-post stannar i mappen Utkorg tills du manuellt initiera en skicka/ta emot-åtgärd i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
