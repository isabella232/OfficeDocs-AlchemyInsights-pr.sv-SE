---
title: Kryptera vissa e-postmeddelanden automatiskt från Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988853"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Kryptera vissa e-postmeddelanden automatiskt från Office 365

1. Välj [E Exchange flödesregler](https://outlook.office365.com/ecp/)i **administrationscentret för e>.** 
2. Klicka på **ikonen Nytt (+)** och sedan på Tillämpa skydd **Meddelandekryptering i Office 365 rättigheter och meddelanden.**
3. Ange **ett** namn för regeln i Namn, till exempel *Kryptera alla meddelanden*.
4. I **Använd den här regeln om** väljer du **[Använd för alla meddelanden]**. 
5. Klicka på **Markera ett bredvid** Gör följande **fält.** 
6. I den **nedrullningsmenyn** för RMS-mallen väljer **du Kryptera** och klickar sedan på **OK.** (Om du inte ser det här alternativet innebär det att din plan inte innehåller automatisk kryptering. Men du kan lägga till den!)
7. Markera **kryssrutan Granska den här regeln med allvarlighetsnivå** och välj sedan önskad nivå. Om ditt företag har avtalsmässiga skyldigheter att skicka krypterade e-postmeddelanden rekommenderar jag att ställa in nivån **på Hög.**
8. Klicka **på Framtvinga under Välj** en modell för **regeln.** 
9. Välj valfritt val (i en lista med valfria val som du kan göra i det här läget. Många av dem kan lämnas med standardinställningen för enkelhetens skull).
10. Klicka på **Spara**.

> [!IMPORTANT]
> Du kan alltid gå tillbaka och redigera regeln senare.

Mer information om hur du skapar regler för kryptering finns i Definiera [e-postflödesregler för att kryptera e-postmeddelanden i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

