---
title: Flera objekt har samma e-postadress som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439709"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Flera objekt har samma e-postadress som identitet

**Flera objekt**

En av de vanligaste orsakerna till det här felet är att inte kunna dirigera en Outlook Web Access-begäran korrekt i närvaro av flera objekt som har samma e-postadress som identitet. Om du vill söka efter dessa objekt kör du följande kommandon:

· Mottagare<email address>

· Hämta användare<email address>

· Get-User <email address> -SoftDeletedUser

· Få kontakt<email address>

· Hämta-postlåda <email address> -PublicFolder

· Hämta brevlåda <email address> -IncludeSoftDeletedMailbox

· Hämta brevlåda <email address> -InaktivaPostlådandå

Lös problemet genom att ta bort flera objekt med samma e-postidentitet och se till att det finns ett enda objekt med den specifika e-postidentiteten och att mottagaren är UserMailbox.

**Samma adress används för företags- och konsumentbrevlådor**

En annan orsak är när samma adress används för företags- och konsumentpostlådor. I det här fallet måste användaren ändra sitt primära konsumentalias tills Cafe stöder det här scenariot. Detta är ett permanent fel som inte försvinner utan ingripande.

Mer information finns i [Ändra e-postadressen eller telefonnumret för ditt Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).