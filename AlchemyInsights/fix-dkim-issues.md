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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717580"
---
# <a name="fix-dkim-setup-issues"></a>Åtgärda problem med installation av DKIM

Om du får problem med att aktivera DKIM för din anpassade domän gör du så här:

- De flesta DKIM-inställningsproblem är relaterade till felaktiga DNS-poster. Kontrollera att DKIM CNAME-posten **(inte** en TXT-post) är korrekt formaterad. Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- När du har skapat eller uppdaterat dina DKIM DNS-poster på DNS-värdtjänsten för din domän (vanligtvis domänregistratorer) väntar du på att DNS-posterna ska spridas.

- Om du inte kan skapa DKIM DNS-posterna i \<administrationscentret\> kan du ersätta CustomDomain med din anpassade domän (till `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`exempel contoso.com) och köra det här kommandot i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
