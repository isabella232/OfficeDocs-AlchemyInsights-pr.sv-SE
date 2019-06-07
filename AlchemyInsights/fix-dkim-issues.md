---
title: Åtgärda problem vid installation av DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765461"
---
# <a name="fix-dkim-setup-issues"></a>Åtgärda problem vid installation av DKIM

Om du har problem att aktivera DKIM för din egen domän, gör du följande:

- De flesta problem vid installation av DKIM är relaterade till felaktiga DNS-poster. Kontrollera DKIM CNAME-posten (**inte** en TXT-post) är korrekt formaterad. Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- När du skapar eller uppdatera DKIM DNS-poster i DNS-värdtjänsten för din domän (vanligtvis din domänregistrerare), vänta på att sprida DNS-posterna.

- Om du inte kan skapa DKIM DNS-poster i administratörscenter, kan du ersätta \<CustomDomain\> med din egen domän (till exempel contoso.com) och kör detta kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
