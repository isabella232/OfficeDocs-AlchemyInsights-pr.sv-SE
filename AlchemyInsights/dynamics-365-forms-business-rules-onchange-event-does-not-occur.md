---
title: Dynamics 365 utgör affärsregler - affärsregel som utlöser inte för ett formulär
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529037"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-händelsen inträffar inte om fältet ändras programmatiskt

*OnChange* -händelsen inträffar inte om fältet ändras programmatiskt med hjälp av den *attribut.* [SättVärde](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metod. Om du vill använda händelsehanterare för *OnChange* -händelsen att köra efter värdet måste du använda den *attributet formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metod i koden.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
