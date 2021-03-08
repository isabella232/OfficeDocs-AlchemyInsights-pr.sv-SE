---
title: Kryptera vissa e-postmeddelanden i Office 365 automatiskt
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526743"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Kryptera vissa e-postmeddelanden i Office 365 automatiskt

Du kan automatiskt kryptera meddelanden som användare skickar till vissa externa personer eller organisationer. Gör så här:

1. I [administrationscentret för Exchange väljer](https://outlook.office365.com/ecp/)du **e-postflöde > regler.** 
2. Klicka på **ikonen Ny (+)** och sedan på Använd meddelandekryptering **i Office 365 och rättighetsskydd för meddelanden.**
3. Ange **ett** namn för regeln i Namn, till exempel Kryptera meddelanden *som skickas till DrToniRamos@gmail.com.*
4. I **Använd den här regeln om** väljer du > mottagaren är den här **personen.** 
5. I fönstret **Välj medlemmar** väljer du namnet på den person som du vill att krypteringsregeln ska gälla för och klickar sedan på **Lägg till.** 
6. Klicka på OK när du har lagt till **alla användare.**
7. Klicka på **Markera ett fält bredvid** Gör följande **fält.** 
8. I den **nedrullningsmenyn** för RMS-mallen väljer **du** Kryptera och klickar sedan på **OK.** (Om du inte ser det här alternativet innebär det att ditt abonnemang inte innehåller automatisk kryptering. Men du kan lägga till den!)
9. Välj valfritt (i en lista med valfria val som du kan göra i det här läget, där många av dem kan lämnas kvar med standardinställningen för enkelhetens skull).
10. Klicka på **Spara**.

> [!IMPORTANT]
> Du kan alltid gå tillbaka och redigera regeln senare.

Mer information om hur du skapar regler för kryptering finns i [Definiera e-postflödesregler för att kryptera e-postmeddelanden i Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

