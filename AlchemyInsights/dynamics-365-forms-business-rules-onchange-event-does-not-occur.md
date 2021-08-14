---
title: Affärsregler i Dynamics 365 Forms – affärsregel som inte går att skapa ett formulär
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947317"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Händelsen OnChange inträffar inte om fältet ändras programmässigt

Händelsen *OnChange* inträffar inte om fältet ändras programmässigt med hjälp av *attributet.* [sättVärde-metod.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Om du vill att händelsehanterare för *händelsen OnChange* ska köras när du har angett värdet måste du använda *metoden formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) i koden.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
