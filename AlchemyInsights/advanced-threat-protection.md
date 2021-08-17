---
title: Microsoft Defender för Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 0aa2d25952587bdc5e6294870b262116bb7170b38054f91ca1807ebb940ac031
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888976"
---
# <a name="microsoft-defender-for-office-365"></a>Microsoft Defender för Office 365

- Valv Bifogade filer Valv länkar och nätfiskeskydd är en del av Microsoft Defender för Office 365. Enterprise E5, Education A5 och Microsoft 365 Business Premium microsoft Defender för Office 365. Alla andra abonnemang kräver ett tillägg för Microsoft Defender för Office 365 prenumeration.

- Du måste tilldela lämpliga licenser för att skydda användarna med Microsoft Defender för Office 365. Se [Lägga till användare och tilldela licenser samtidigt](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) för anvisningar om hur du mass apply licenses to your users.

- Globala administratörer eller **säkerhetsadministratörer** kan komma åt Microsoft Defender för Office 365-funktioner i Microsoft 365 Defender-portalen på avsnittet E& post och samarbete \> **&** \> **principer för hot.**

- Valv Principer för Valv och länkar kan vara begränsade till specifika domäner, gruppmedlemmar eller enskilda användare. Du kan också ange undantag för Valv och principer Valv länkar baserat på domän, gruppmedlemskap eller enskilda användare.

- Det finns ingen standardprincip Valv för bifogade filer som skyddar e-postmeddelanden. Du måste skapa en [princip för att Valv](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-attachments-policies) skydd för bifogade filer i e-post.

  Valv Bifogade filer SharePoint, OneDrive och Microsoft Teams är aktiverade eller inaktiverade globalt och kräver inte principer Valv för bifogade filer. Mer information finns i Bifoga [Valv för SharePoint, OneDrive och Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/mdo-for-spo-odb-and-teams).

- Det finns ingen standardprincip Valv för länkar som skyddar e-postmeddelanden och Microsoft Teams. Du måste skapa [en princip för att](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies) Valv skydd mot länkar i e-Teams.

  Valv Länkskydd för Office 365-appar tillämpas på alla användare i organisationen som är licensierade för Defender för Office 365, oavsett om användarna ingår i aktiva Valv-länkar eller inte. Mer information finns i inställningar [Valv länkar för Office 365 appar](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links#safe-links-settings-for-office-365-apps).
