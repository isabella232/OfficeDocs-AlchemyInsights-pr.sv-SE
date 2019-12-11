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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959512"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan inte ansluta till gemensamma mappar

Om åtkomst till gemensamma mappar inte fungerar för få användare kan du prova följande:

Anslut till EXO PowerShell och konfigurera DefaultPublicFolderMailbox på problem användarkontot så att det matchar ett på ett fungerande användarkonto.

Exempel:

Hämta postlåda WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Ange postlåda ProblemUser-DefaultPublicFolderMailbox \<värde från föregående kommando>

Vänta minst en timme innan ändringen träder i kraft.