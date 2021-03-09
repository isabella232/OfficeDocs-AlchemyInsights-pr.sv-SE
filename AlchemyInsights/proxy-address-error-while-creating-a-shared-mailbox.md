---
title: Proxyadressfel när en delad postlåda skapas
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568308"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxyadressfel när en postlåda eller ett annat e-postaktivat objekt skapas

Om du försökte skapa ett e-postaktivat objekt (postlåda, delad postlåda osv.) och fick felmeddelandet "Proxyadressen "SMTP:alias@domain.com" används redan...", används den e-postadress du valde redan av ett annat e-postaktivat objekt i organisationen.
  
Du måste hitta den användare, grupp, delade postlåda eller gemensamma mapp som har den här e-postadressen och ta bort den eller ändra dess e-postadress. Sedan kan du skapa ett nytt e-postaktiverat objekt med den lediga e-postadressen. Använd Sök på startsidan för att hitta den. Du kan också använda följande Exchange Online PowerShell-kommando för att söka efter det:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Om du inte vill ta bort den befintliga e-postadressen väljer du en ny e-postadress för det nya objektet du skapar.
  