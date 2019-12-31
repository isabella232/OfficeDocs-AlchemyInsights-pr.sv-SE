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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="22f1d-102">Åtkomst till BitLocker-återställningsnycklar</span><span class="sxs-lookup"><span data-stu-id="22f1d-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="22f1d-103">När du konfigurerar BitLocker-inställningar för Intune Endpoint Protection-princip är det möjligt att definiera om BitLocker-återställningsinformation ska lagras i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="22f1d-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="22f1d-104">Om den här inställningen är konfigurerad bör lagrade återställningsdata vara synlig för en Intune-administratör som en del av enheten registrera data i Intune-enheter bladet på två sätt:</span><span class="sxs-lookup"><span data-stu-id="22f1d-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="22f1d-105">Enheter-Azure AD-enheter-> "enhet" eller enheter-> alla enheter-> "enhet"-> återställningsnycklar</span><span class="sxs-lookup"><span data-stu-id="22f1d-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="22f1d-106">Alternativt, om det finns administrativ åtkomst till själva enheten, kan återställningsnyckeln (lösenord) ses genom att köra följande kommando från en upphöjd kommandotolk:</span><span class="sxs-lookup"><span data-stu-id="22f1d-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="22f1d-107">Om enheten krypterades före registreringen i Intune, kan återställningsnyckeln ha associerats med "Microsoft Account" (MSA) som används för att logga in på enheten under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="22f1d-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="22f1d-108">Om så var fallet bör åtkomst https://onedrive.live.com/recoverykey och inloggning med det MSA Visa de enheter för vilka återställningsnycklar lagrades.</span><span class="sxs-lookup"><span data-stu-id="22f1d-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="22f1d-109">Om enheten krypterades som ett resultat av konfigurationen via domänbaserad Grupprincip, kan återställningsinformationen lagras i den lokala Active Directory.</span><span class="sxs-lookup"><span data-stu-id="22f1d-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

