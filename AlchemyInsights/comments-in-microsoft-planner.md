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
ms.openlocfilehash: 0d87d8c9fafe49de02b9c0158144287c77339886cdb910e006296eac73a2c497
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995531"
---
# <a name="comments-in-microsoft-planner"></a>Kommentarer i Microsoft Planner

Kommentarer om uppgifter i en plan lagras i Exchange Online-postlådan för Microsoft 365-gruppen som är kopplad till planen.  När du lägger till en kommentar i en uppgift skickas ett e-postmeddelande till gruppinkorgen och du får ett e-postmeddelande för varje efterföljande kommentar om uppgiften.

Här är några svar på vanliga problem som rör kommentarer:

- **Användare får inte e-postmeddelanden**– Kommentarer skickas till gruppinkorgen för gruppen som planen tillhör. För att en användare ska ta emot gruppmeddelanden måste gruppen konfigureras att skicka gruppkonversationer till medlemmarnas inkorgar.

- **Kommentarer sparas inte** – Användaren som lägger till kommentaren har inte behörighet att skicka e-post till Microsoft 365-gruppen. Läs [Så här fungerar Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) om du vill ha mer information om det här scenariot.

- Felet **Du har inte längre åtkomst** visas eller **gästanvändare kan inte lägga till kommentarer** – Gästanvändare som inte kan skicka e-post till gruppinkorgen kan se det här meddelandet. Lös problemet genom att se till att gästanvändaren har en giltig e-postadress.

- **Borttagna användare får e-postmeddelanden** – Om en användare kommenterar en uppgift innan hen tas bort från planen inkluderar e-posttråden användarna för alla kommentarer som skrivs om uppgiften.

Mer information om kommentarer i Microsoft Planner finns i [Så här fungerar Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) och [Kommentera uppgifter i Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
