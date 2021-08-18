---
title: Full NDR i AggregateGroupMailbox för e-post som skickas Microsoft 365 e-postgrupp
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315928"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Full NDR i AggregateGroupMailbox för e-post som skickas Microsoft 365 e-postgrupp

Använd följande EXO Shell-kommando för att skapa en Exchange-transportregel för att tyst släppa e-postmeddelanden som skickas till aggregerad grupppostlåda:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Obs!** Ersätt SMTP-adressen i **-SentTo med SMTP-adressen** för den samlade grupppostlådan i klientorganisationen. Du kan hämta SMTP-adressen för den samlade grupppostlådan från den NDR-post som tagits emot.



