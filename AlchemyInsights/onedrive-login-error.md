---
title: Fel i OneDrive-AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982547"
---
# <a name="onedrive-login-error-aadsts50011"></a>Fel i OneDrive-AADSTS50011

Om du får ett fel meddelande om att svars-URL: en som angetts i begäran inte matchar svaret "när du loggar in på OneDrive-appen, kan du kontrol lera följande:

Din OneDrive-version måste vara lika med eller större än version 20.052. XXXX. XXXX. Kontrol lera din version genom att klicka på den blå OneDrive-ikonen i meddelande fältet, Välj **hjälp & inställningar > inställningar > om**.

Nätverket kan blockera trafik till **g.live.com** och **oneclient.SFX.MS**. Om den trafiken är blockerad kan OneDrive inte uppdatera sig själv. Arbeta med nätverks administratören för att se till att du har åtkomst till dessa URL: er. [Dessa slut punkter](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) bör kunna nås för kunder som använder Microsoft 365-abonnemang.

Om du behöver skaffa en aktuell version av OneDrive manuellt kan du gå till [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
