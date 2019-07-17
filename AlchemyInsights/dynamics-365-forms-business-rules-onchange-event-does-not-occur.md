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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748903"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="fb005-102">OnChange-händelsen inträffar inte om fältet ändras programmatiskt</span><span class="sxs-lookup"><span data-stu-id="fb005-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="fb005-103">*OnChange* -händelsen inträffar inte om fältet ändras programmatiskt med hjälp av den *attribut.* [SättVärde](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metod.</span><span class="sxs-lookup"><span data-stu-id="fb005-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="fb005-104">Om du vill använda händelsehanterare för *OnChange* -händelsen att köra efter värdet måste du använda den *attributet formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metod i koden.</span><span class="sxs-lookup"><span data-stu-id="fb005-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
