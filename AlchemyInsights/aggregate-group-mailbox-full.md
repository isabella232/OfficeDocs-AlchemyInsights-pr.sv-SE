---
title: AggregateGroupMailbox full NDR mottaget för e-post som skickas till Microsoft 365-gruppen
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722078"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox full NDR mottaget för e-post som skickas till Microsoft 365-gruppen

Använd följande EXO Shell-kommando för att skapa en Exchange-transportprovidern för att direkt släppa e-postmeddelanden som skickas till grupp post lådan:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Ersätt SMTP-adressen i **-SentTo** med SMTP-adressen till grupp post lådan i klient organisationen. Du kan hämta SMTP-adressen för den aggregerade gruppens post låda från rapporten.



