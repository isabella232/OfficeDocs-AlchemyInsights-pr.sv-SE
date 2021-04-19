---
title: Kommentarer i Microsoft Planner
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
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817658"
---
# <a name="comments-in-microsoft-planner"></a>Kommentarer i Microsoft Planner

Kommentarer om uppgifter i en plan lagras i Exchange Online-postlådan för Microsoft 365-gruppen som är kopplad till planen.  När du lägger till en kommentar i en uppgift skickas ett e-postmeddelande till gruppinkorgen och du får ett e-postmeddelande för varje efterföljande kommentar om uppgiften.

Här är några svar på vanliga problem som rör kommentarer:

- **Användare får inte e-postmeddelanden**– Kommentarer skickas till gruppinkorgen för gruppen som planen tillhör. För att en användare ska ta emot gruppmeddelanden måste gruppen konfigureras att skicka gruppkonversationer till medlemmarnas inkorgar.

- **Kommentarer sparas inte** – Användaren som lägger till kommentaren har inte behörighet att skicka e-post till Microsoft 365-gruppen. Läs [Så här fungerar Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) om du vill ha mer information om det här scenariot.

- Felet **Du har inte längre åtkomst** visas eller **gästanvändare kan inte lägga till kommentarer** – Gästanvändare som inte kan skicka e-post till gruppinkorgen kan se det här meddelandet. Lös problemet genom att se till att gästanvändaren har en giltig e-postadress.

- **Borttagna användare får e-postmeddelanden** – Om en användare kommenterar en uppgift innan hen tas bort från planen inkluderar e-posttråden användarna för alla kommentarer som skrivs om uppgiften.

Mer information om kommentarer i Microsoft Planner finns i [Så här fungerar Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) och [Kommentera uppgifter i Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
