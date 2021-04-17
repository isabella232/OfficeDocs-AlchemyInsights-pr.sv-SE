---
title: BitLocker-återställningsnycklar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820304"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Komma åt Bitlocker-återställningsnycklar

När du konfigurerar Bitlocker-inställningar Intune Endpoint Protection Policy kan du definiera om Bitlocker-återställningsinformation ska lagras i Azure Active Directory.

Om den inställningen är konfigurerad bör lagrade återställningsdata vara synliga för en Intune-administratör som en del av enhetspostdata i bladet Intune-enheter på två sätt:

Enheter - Azure AD-enheter -> "Enhet" ELLER Enheter -> Alla enheter -> "Enhet" -> Återställningsnycklar

Alternativt, om det finns administrativ åtkomst till själva enheten, kan återställningsnyckeln (Lösenord) visas genom att köra följande kommando från en upphöjd kommandotolk:

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
Om enheten krypterades före registrering i Intune kan återställningsnyckeln ha kopplats till det Microsoft-konto (MSA) som används för att logga in på enheten under OOBE-processen. Om så är fallet bör åtkomst till och inloggning med det MSA-programmet visa de enheter  https://onedrive.live.com/recoverykey som återställningsnycklar lagrades för.
 
Om enheten krypterades på grund av konfiguration genom domänbaserad grupprincip kan återställningsinformationen lagras på den lokala distributionen av Active Directory.

Om du har konfigurerat Slutpunktsskyddsprincip att lagra återställningsnyckeln i Azure Active Directory men nyckeln för en viss enhet inte har laddats upp kan du utlösa överföringen genom att rotera återställningsnyckeln för enheten från MEM-konsolen. Mer information finns i [Rotera BitLocker-återställningsnycklar.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

