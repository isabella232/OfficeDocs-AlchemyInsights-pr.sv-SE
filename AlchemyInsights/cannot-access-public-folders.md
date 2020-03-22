---
title: Det går inte att komma åt gemensamma mappar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891767"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Det går inte att ansluta till gemensamma mappar

Om åtkomst till gemensamma mappar inte fungerar för vissa användare kan du prova följande:

Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox på problemet användarkontot så att den matchar parametern på ett fungerande användarkonto.

Exempel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox-värde \<från föregående kommando>

Vänta minst en timme innan ändringen börjar gälla.

Om problemet kvarstår följer du [den här proceduren](https://aka.ms/pfcte) för att felsöka problem med åtkomst till gemensamma mappar med Outlook.