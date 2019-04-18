---
title: Säkerhetsetiketter visas inte
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: fac86806ac6931d7c69eaa7b6321c87f8c21ce26
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909597"
---
# <a name="sensitivity-labels-not-appearing"></a>Säkerhetsetiketter visas inte

Säkerhetsetiketter kan du klassificera och skydda känsliga innehåll. Om du vill veta mer om den här funktionen finns i [Översikt över säkerhetsetiketter](https://docs.microsoft.com/en-us/office365/securitycompliance/sensitivity-labels).

Om du har konfigurerat din säkerhetsetiketter, men de visas inte i Office-program, kontrollerar du följande:

- Kontrollera att etiketten känslighet har [publicerats](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) till användare och grupper som du vill.

- Bekräfta att användaren använder en app som stöder säkerhetsetiketter - Se [känslighet etiketter i dokumentet](https://support.office.com/en-us/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).
 
 
- Om du inte [migrerar Azure informationsskydd etiketter](https://docs.microsoft.com/en-us/azure/information-protection/configure-policy-migrate-labels)kan vara medveten om de överväganden anges [här](https://docs.microsoft.com/en-us/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Förhindra dataförlust (DLP) stöder: för närvarande endast behålla etiketter kan användas som ett villkor i DLP-principer.  Stöd för säkerhetsetiketter i en DLP-princip är inte tillgänglig ännu, men vi arbetar med den.

Mer information om möjliga problem finns [kända problem med säkerhetsetiketter](https://support.office.com/en-us/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US).