---
title: BitLocker-återställningsnycklar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908832"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Åtkomst till BitLocker-återställningsnycklar

När du konfigurerar BitLocker-inställningar för Intune Endpoint Protection-princip är det möjligt att definiera om BitLocker-återställningsinformation ska lagras i Azure Active Directory.

Om den här inställningen är konfigurerad bör lagrade återställningsdata vara synlig för en Intune-administratör som en del av enheten registrera data i Intune-enheter bladet på två sätt:

Enheter-Azure AD-enheter-> "enhet" eller enheter-> alla enheter-> "enhet"-> återställningsnycklar

Alternativt, om det finns administrativ åtkomst till själva enheten, kan återställningsnyckeln (lösenord) ses genom att köra följande kommando från en upphöjd kommandotolk:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Om enheten krypterades före registreringen i Intune, kan återställningsnyckeln ha associerats med "Microsoft Account" (MSA) som används för att logga in på enheten under OOBE-processen. Om så var fallet bör åtkomst https://onedrive.live.com/recoverykey och inloggning med det MSA Visa de enheter för vilka återställningsnycklar lagrades.
 
Om enheten krypterades som ett resultat av konfigurationen via domänbaserad Grupprincip, kan återställningsinformationen lagras i den lokala Active Directory.
 

