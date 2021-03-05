---
title: Hitta händelser som utförs för inkorgsregler
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483705"
---
# <a name="find-events-performed-on-inbox-rules"></a>Hitta händelser som utförs för inkorgsregler

När regler för Inkorgen skapas, ändras eller tas bort registreras händelserna i granskningsloggen. Så här granskar du dem:

1. Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj Sök > granskningsloggsökning.

    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Markera fältet Aktiviteter och sök efter Aktiviteter i Exchange-postlådan och välj sedan New-InboxRule skapa inkorgsregel från Outlook Web App. När du är klar klickar du utanför fönstret för att minimera fönstret Aktiviteter.
1. Ange datumintervallet och välj sedan användarnamnet för den användare du vill undersöka i fältet Användare. Du kan välja flera användare åt gången.
1. Välj Sök. Aktiviteterna visas under Resultat.
1. Om du vill visa information väljer du en aktivitet och sedan Mer information. Under avsnittet Parametrar ser du namnet på regeln, villkorsuppsättningen och de åtgärder som regeln kommer att vidta.

Mer information finns i Söka i Office 365-granskningsloggen för att felsöka vanliga scenarier.