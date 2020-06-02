---
title: Åtgärda problem med installation av DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506792"
---
# <a name="fix-dkim-setup-issues"></a>Åtgärda problem med installation av DKIM

Om du får problem med att aktivera DKIM för din anpassade domän gör du så här:

- De flesta DKIM-inställningsproblem är relaterade till felaktiga DNS-poster. Kontrollera att DKIM CNAME-posten **(inte** en TXT-post) är korrekt formaterad. Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- När du har skapat eller uppdaterat dina DKIM DNS-poster på DNS-värdtjänsten för din domän (vanligtvis domänregistratorer) väntar du på att DNS-posterna ska spridas.

- Om du inte kan skapa DKIM DNS-posterna i administrationscentret kan du ersätta \<CustomDomain\> med din anpassade domän (till exempel contoso.com) och köra det här kommandot i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
