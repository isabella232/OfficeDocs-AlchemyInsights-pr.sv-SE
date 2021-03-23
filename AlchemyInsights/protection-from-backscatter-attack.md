---
title: Skydd mot bakåtcatterattack
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037180"
---
# <a name="protection-from-backscatter-attack"></a>Skydd mot bakåtcatterattack

Bakåtcatter är rapporter om utebliven leverans (kallas även NDR-rapporter eller icke-leveranskända meddelanden) som du får för meddelanden som du inte har skickat. Skräppostavs spammare förfalskar meddelandens adress **från:** och de använder ofta riktiga e-postadresser för att låna ut trovärdigheten för sina meddelanden. Så om skräppostavsändare oundvikligen skickar meddelanden till mottagare som inte finns, luras nämligen mål-e-postservern i princip att skicka tillbaka det olevererbara meddelandet i en NDR till den förfalskade avsändaren i **Från:-adressen.**

Ytterligare information finns i [Bakåtcatter i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**Aktivera skydd mot bakåtcatter**

Aktivera bakåtcatterskydd genom att följa sökvägen nedan.

**protection.office.com > Threat Management > Policy > Antispam > Välj policyn för skräppostfilter och redigera principen > Egenskaper för skräppost > Markera som skräppost > NDR-bakåtcatter > Ställ in den på "På"**

Läs följande om du tror att ett konto har komprometterats:

- [Hantera ett komprometterat e-postkonto](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Ta bort blockerade användare från portalen begränsade användare i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



