---
title: Åtgärda problem med DKIM konfiguration
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744968"
---
# <a name="fix-dkim-setup-issues"></a>Åtgärda problem med DKIM konfiguration

Om du får problem med att aktivera DKIM för din anpassade domän gör du följande:

- De flesta DKIM installations problem är relaterade till felaktiga DNS-poster. Verifiera att DKIM CNAME-posten (**inte** en TXT-post) är korrekt formaterad. Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- När du har skapat eller uppdaterat dina DKIM DNS-poster hos DNS-värd för din domän (vanligt vis domän registratorn) väntar du på att DNS-posterna ska spridas.

- Om du inte kan skapa DNS-posterna för DKIM i administrations centret kan du ersätta \<CustomDomain\> med din egen domän (till exempel contoso.com) och köra det här kommandot i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
