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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232648"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Åtgärda meddelanden som har fastnat i utkorgen

Vi rekommenderar att du börjar med att köra scenariot ["Jag har problem med att skicka, ta emot eller hitta e-postmeddelanden"](https://aka.ms/SaRA-OutlookSendReceive) från microsoft [support- och återställningsassistenten](https://diagnostics.office.com/#/) på den berörda datorn.

När ett meddelande fastnar i utkorgen är den troligaste orsaken en stor bilaga eller alternativet "Skicka omedelbart när du är ansluten" är inte aktiverat.

**Ta bort den stora bilagan**

1. Klicka på **Skicka/ta emot** > **arbete offline**. 
2. Klicka på Utkorgen i **navigeringsfönstret**. Härifrån kan du: 
    - Ta bort meddelandet. Välj den och klicka på **Ta bort.**
    - Dra meddelandet till **utkastmappen,** dubbelklicka för att öppna meddelandet och ta bort den bifogade filen (klicka på den och klicka på **Ta bort).**
3. Om ett fel talar om för dig att Outlook försöker överföra meddelandet stänger du Outlook. Det kan ta en stund att avsluta. Om Outlook inte stängs trycker du på **Ctrl+Alt+Delete** och klickar på **Starta Aktivitetshanteraren**. I **Aktivitetshanteraren** väljer du fliken Processer, rullar ned till outlook.exe och klickar på **Avsluta process**.
4. När Outlook har stängts startar du om Outlook och upprepar steg 2-3. 
5. När du har tagit bort den bifogade filen klickar du på **Skicka/ta emot** > **arbete offline** för att avmarkera knappen och fortsätta arbeta online. 

Meddelanden fastnar också i utkorgen när du klickar på **Skicka**, men du är inte ansluten. Klicka på **Skicka/ta emot** och titta på knappen **Arbeta offline.** Om den är blå är du frånkopplad. Klicka på den för att ansluta (knappen blir vit) och klicka på **Skicka alla**.
 
**Aktivera Skicka direkt när du är ansluten**
 
1. Klicka på **Alternativ**på fliken Arkiv .

2. Klicka på **Avancerat**i dialogrutan Outlook-alternativ .

3. I avsnittet Skicka och ta emot klickar du för att aktivera **Skicka direkt när du är ansluten**. Klicka på **OK**.
 
För fullständig information, se:
- [Video: Skicka eller ta bort ett fast e-postmeddelande](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-post finns kvar i mappen Utkorgen tills du initierar en skicka/ta-mottagning i Outlook manuellt](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
