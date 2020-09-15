---
title: Identifiera händelser för ta bort meddelanden i gransknings loggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696531"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Gransknings loggar för borttagna e-postmeddelanden

Från och med den 2019 januari aktiverar Microsoft automatiskt gransknings loggning för post låda. Om du till exempel vill ta bort meddelande händelser för en viss användare måste du manuellt aktivera borttagnings åtgärderna för granskning. Om gransknings loggning för post lådor är aktiverat för din organisation eller för en viss användare följer du stegen nedan.

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klicka på **Sök och** granska och välj **gransknings loggs ökning**.

3. Välj datum intervall i fälten **start datum** och **slutdatum** . Ange användar namn för den användare som du vill undersöka (användaren som tog bort objekten). I fältet **aktiviteter** väljer du **borttagna meddelanden från mappen Borttaget** och **flyttade meddelanden till mappen Borttaget**.

4. Klicka på **Sök**.

Välj en gransknings post i resultatet. I den utfällbara informationen klickar du på **Mer information**. Ytterligare information om det borttagna objektet (till exempel raden ämne och platsen för objektet när det togs bort) visas i fältet **AffectedItems** . Egenskapen **ClientInfoString** visar om borttagningen skedde i Outlook, Outlook på webben (tidigare Outlook Web App) eller annan enhet.

Mer information finns i [bestämma vem som konfigurerar e-postvidarebefordran för en post låda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Obs!** du kan inte hämta borttagna objekt med hjälp av Gransknings logg funktionen. Information om hur du hämtar borttagna meddelanden i Outlook på webben finns i [återställa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
