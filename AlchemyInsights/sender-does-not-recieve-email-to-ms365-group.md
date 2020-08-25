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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="a0bec-102">Avsändaren får inte e-post som skickas till Microsoft 365-gruppen</span><span class="sxs-lookup"><span data-stu-id="a0bec-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="a0bec-103">Som standard får avsändaren av ett e-postmeddelande till en Microsoft 365-grupp inte en kopia av meddelandet i sin inkorg, även om avsändaren är medlem i gruppen.</span><span class="sxs-lookup"><span data-stu-id="a0bec-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="a0bec-104">Använd det här EXO PowerShell-kommandot för att låta avsändaren få en kopia av varje e-postmeddelande de skickar till gruppen Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="a0bec-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="a0bec-105">Så här aktiverar du inställningen för alla post lådor samtidigt:</span><span class="sxs-lookup"><span data-stu-id="a0bec-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="a0bec-106">**Obs!** Ändringar av den här inställningen tar upp till en timme att träda i kraft.</span><span class="sxs-lookup"><span data-stu-id="a0bec-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>