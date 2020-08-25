---
title: Avsändaren får inte e-post som skickas till Microsoft 365-gruppen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872208"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Avsändaren får inte e-post som skickas till Microsoft 365-gruppen

Som standard får avsändaren av ett e-postmeddelande till en Microsoft 365-grupp inte en kopia av meddelandet i sin inkorg, även om avsändaren är medlem i gruppen.

Använd det här EXO PowerShell-kommandot för att låta avsändaren få en kopia av varje e-postmeddelande de skickar till gruppen Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Så här aktiverar du inställningen för alla post lådor samtidigt:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Obs!** Ändringar av den här inställningen tar upp till en timme att träda i kraft.