---
title: Gruppen skicka som Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872210"
---
# <a name="send-as-microsoft-365-group"></a>Gruppen skicka som Microsoft 365

Du kan tilldela Send As-behörigheter för att tillåta specifika användare att skicka meddelanden som en Microsoft 365-grupp:  

1. Ansluta till Exchange Online PowerShell.  

2. Kör följande kommando:  

    RecipientPermission- `<GroupName>` förlitare `<MailboxName>` -AccessRights-skickare

Mer information finns i [tillåta medlemmar att skicka som eller skicka för en grupp](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).