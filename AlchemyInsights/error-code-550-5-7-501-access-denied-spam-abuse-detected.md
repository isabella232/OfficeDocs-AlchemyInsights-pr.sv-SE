---
title: Felkod 550 5.7.501 Åtkomst nekades, skräppostfel upptäcktes
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044286"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Åtkomst nekades, skräppost missbruk upptäcktes

Vanligtvis visas det här meddelandet när användare skickar e-postmeddelanden från IP-adresser med hjälp av den ursprungliga *.onmicrosoft.com-domänen* som tilldelas till nya klientorganisationar i Microsoft 365. Det enklaste sättet att lösa det här problemet är att:

1. [Lägg till en domän i klientorganisationen.](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)

2. [Ändra användarnas primära e-postadress till](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) den nya anpassade domänen som du just lagt till.
