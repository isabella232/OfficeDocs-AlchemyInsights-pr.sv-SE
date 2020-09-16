---
title: Känslighets etiketter visas inte
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801202"
---
# <a name="sensitivity-labels-not-appearing"></a>Känslighets etiketter visas inte

Med känslighets etiketter kan du klassificera och skydda känsligt innehåll. De kan skapas i Microsoft 365 Compliance Center, Microsoft 365 säkerhets Center eller Microsoft 365 Security & Support Center under klassificerings > känslighets etiketter. Mer information om den här funktionen finns i [Översikt över känslighets etiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Om du har konfigurerat dina känslighets etiketter men inte visas i Microsoft 365-apparna kontrollerar du följande:

- Kontrol lera att känslighets etiketten har [publicerats](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) till de användare och grupper som du vill använda.

- Bekräfta att användaren använder ett program som stöder känslighets etiketter – se [känslighets etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Om du [migrerar etiketter för Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)bör du tänka på de överväganden som visas [här](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Stöd för data förlust skydd (DLP): just nu kan endast bevarande etiketter användas som villkor i DLP-principer.  Stöd för känslighets etiketter i en DLP-princip är ännu inte tillgängligt, men vi jobbar på det.

- När kryptering är aktiverat för en känslighets etikett kan du välja mellan:
    - Tilldela behörigheter nu
    - Låta användare tilldela behörigheter


Mer information om möjliga problem finns i [kända problem med känslighets etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).