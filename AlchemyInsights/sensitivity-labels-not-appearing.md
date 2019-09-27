---
title: Känslighets etiketter visas inte
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207243"
---
# <a name="sensitivity-labels-not-appearing"></a>Känslighets etiketter visas inte

Med hjälp av känslighets etiketter kan du klassificera och skydda känsligt innehåll. De kan skapas i Microsoft 365 Efterlevnadscenter, Microsoft 365 Security Center eller Office 365 Security & regelefterlevnadscenter under klassificering > känslighets etiketter. Mer information om den här funktionen finns [i Översikt över känslighets etiketter](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Om du har konfigurerat känslighets etiketterna men inte visas i Office-apparna kontrollerar du följande:

- Kontrollera att känslighets etiketten har [publicerats](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) till de användare och grupper som du vill ha.

- Kontrollera att användaren använder en app som stöder känslighets etiketter-se [känslighets etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Om du [migrerar Azure information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), vara medveten om de överväganden som anges [här](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Stöd för data förlust skydd (DLP): för närvarande kan endast lagrings etiketter användas som ett villkor i DLP-principer.  Stöd för känslighet etiketter i en DLP-princip är inte tillgänglig ännu men vi arbetar på den.

- När kryptering är aktiverat på en känslighetsetikett kan du välja att antingen:
    - Tilldela behörigheter nu
    - Låt användarna tilldela behörigheter


Mer information om möjliga problem finns i [kända problem med känslighets etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).