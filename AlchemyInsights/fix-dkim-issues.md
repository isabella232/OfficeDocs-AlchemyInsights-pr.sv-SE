---
title: Åtgärda DKIM-konfigurationsproblem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945949"
---
# <a name="fix-dkim-setup-issues"></a>Åtgärda DKIM-konfigurationsproblem

Om du får problem med att aktivera DKIM för din anpassade domän gör du så här:

- De flesta DKIM-konfigurationsproblem är relaterade till felaktiga DNS-poster. Verifiera att DKIM CNAME-posten **(inte** en TXT-post) är rätt formaterad. Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- När du har skapat eller uppdaterat DKIM DNS-posterna hos DNS-värdtjänsten för domänen (vanligtvis din domänregistrator) väntar du tills DNS-posterna har spridits.

- Om du inte kan skapa DKIM DNS-posterna i administrationscentret kan du ersätta med din egen domän (till exempel contoso.com) och köra det här kommandot \<CustomDomain\> [i Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
