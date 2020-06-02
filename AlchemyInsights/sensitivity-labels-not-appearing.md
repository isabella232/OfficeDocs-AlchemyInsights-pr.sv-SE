---
title: Känslighetsetiketter visas inte
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511670"
---
# <a name="sensitivity-labels-not-appearing"></a>Känslighetsetiketter visas inte

Med känslighetsetiketter kan du klassificera och skydda ditt känsliga innehåll. De kan skapas i Microsoft 365 compliance center, Microsoft 365 security center eller Microsoft 365 security & Compliance Center under Klassificering > känslighetsetiketter. Mer information om den här funktionen finns i [Översikt över känslighetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Om du har konfigurerat känslighetsetiketterna men inte visas i Office-programmen kontrollerar du följande:

- Bekräfta att känslighetsetiketten har [publicerats](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) för de användare och grupper som du vill använda.

- Bekräfta att användaren använder en app som stöder känslighetsetiketter – se [känslighetsetiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Om du [migrerar Azure Information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)bör du vara medveten om de överväganden som anges [här](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- DLP-stöd (Data loss prevention) : För närvarande kan endast kvarhållningsetiketter användas som ett villkor i DLP-principer.  Stöd för känslighetsetiketter i en DLP-princip är inte tillgängligt ännu, men vi arbetar på det.

- När kryptering är aktiverat på en känslighetsetikett kan du välja att antingen:
    - Tilldela behörigheter nu
    - Låta användare tilldela behörigheter


Mer information om möjliga problem finns i [Kända problem med känslighetsetiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).