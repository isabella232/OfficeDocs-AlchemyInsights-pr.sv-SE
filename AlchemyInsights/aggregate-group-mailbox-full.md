---
title: Full NDR i AggregateGroupMailbox för e-post som Microsoft 365 till Microsoft 365 postgrupp
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951871"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Full NDR i AggregateGroupMailbox för e-post som Microsoft 365 till Microsoft 365 postgrupp

Använd följande EXO Shell-kommando för att skapa en Exchange för att tyst släppa e-postmeddelanden som skickas till aggregerad grupppostlåda:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Ersätt SMTP-adressen i **-SentTo med** SMTP-adressen för den samlade grupppostlådan i klientorganisationen. Du kan hämta SMTP-adressen för den samlade grupppostlådan från den NDR-post som tagits emot.



