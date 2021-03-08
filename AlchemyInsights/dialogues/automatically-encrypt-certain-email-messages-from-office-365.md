---
title: Kryptera vissa e-postmeddelanden från Office 365 automatiskt
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526765"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Kryptera vissa e-postmeddelanden från Office 365 automatiskt

1. I [administrationscentret för Exchange väljer](https://outlook.office365.com/ecp/)du **e-postflöde > regler.** 
2. Klicka på **ikonen Ny (+)** och sedan på Använd meddelandekryptering **i Office 365 och rättighetsskydd för meddelanden.**
3. Ange **ett** namn på regeln i Namn, till exempel *Kryptera alla meddelanden.*
4. I **Använd den här regeln om** väljer du **[Använd för alla meddelanden]**. 
5. Klicka på **Markera ett fält bredvid** Gör följande **fält.** 
6. I den **nedrullningsmenyn** för RMS-mallen väljer **du** Kryptera och klickar sedan på **OK.** (Om du inte ser det här alternativet innebär det att ditt abonnemang inte innehåller automatisk kryptering. Men du kan lägga till den!)
7. Markera kryssrutan **Granska denna regel med allvarlighetsnivå** och välj sedan önskad nivå. Om ditt företag har avtalsenliga skyldigheter att skicka krypterade e-postmeddelanden rekommenderar jag att du sätter nivån till **Hög.**
8. Klicka **på Tillämpa under Välj en** modell för den här **regeln.** 
9. Välj valfritt (i en lista med valfria val som du kan göra i det här läget, där många av dem kan lämnas kvar med standardinställningen för enkelhetens skull).
10. Klicka på **Spara**.

> [!IMPORTANT]
> Du kan alltid gå tillbaka och redigera regeln senare.

Mer information om hur du skapar krypteringsregler finns i [Definiera e-postflödesregler för att kryptera e-postmeddelanden i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

