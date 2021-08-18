---
title: Kryptera e-Office 365 som skickas till vissa domäner automatiskt
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318866"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Kryptera e-Office 365 som skickas till vissa domäner automatiskt

1. I [administrationscentret Exchange du](https://outlook.office365.com/ecp/)E-postflödesregler **>**. 
2. Klicka på **ikonen Nytt (+)** och sedan på Tillämpa skydd **Meddelandekryptering i Office 365 rättigheter och meddelanden.**
3. Ange **ett** namn på regeln i Namn, till exempel Kryptera meddelanden *som skickas till contoso.com*.
4. I **Använd den här regeln om** väljer du mottagaren > domän **är**. 
5. Ange namnet på domänen, till exempel **contoso.com**.
6. Klicka på **ikonen Lägg till (+)** och sedan på **OK.**
7. Klicka på **Markera ett bredvid** Gör följande **fält.** 
8. I den **nedrullningsmenyn** för RMS-mallen väljer **du Kryptera** och klickar sedan på **OK.** (Om du inte ser det här alternativet innebär det att din plan inte innehåller automatisk kryptering. Men du kan lägga till den!)
9. Välj valfritt val (i en lista med valfria val som du kan göra i det här läget. Många av dem kan lämnas med standardinställningen för enkelhetens skull).
10. Klicka på **Spara**.

**Viktigt:** Du kan alltid gå tillbaka och redigera den här regeln senare.

Mer information om hur du skapar regler för kryptering finns i Definiera [e-postflödesregler för att kryptera e-postmeddelanden i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)