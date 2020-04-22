---
title: Åtgärda problem med e-postleverans på e-postaktiverade gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716370"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Åtgärda problem med e-postleverans på e-postaktiverade gemensamma mappar

Om externa avsändare inte kan skicka meddelanden till dina e-postaktiverade gemensamma mappar och avsändarna får **felmeddelandet: det gick inte att hitta (550 5.4.1)** kontrollerar du att e-postdomänen för den gemensamma mappen är konfigurerad som en intern relay-domän i stället för en auktoritär domän:

1. Öppna [Administrationscentret för Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå till **Domäner för** **e-postflöde** \> Accepterade, välj den accepterade domänen och klicka sedan på **Redigera**.

3. Om domäntypen är inställd på **Auktoritär**på egenskapssidan som öppnas ändrar du värdet till **Internt relä** och klickar sedan på **Spara**.

Om externa avsändare får felet **som du inte har behörighet (550 5.7.13)** kör du följande kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) för att se behörigheterna för anonyma användare i den gemensamma mappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Om du vill att externa användare ska kunna skicka e-post till den här gemensamma mappen lägger du till åtkomsten till CreateItems till användaren Anonym. Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
