---
title: Korrigera problem med e-postleverans till e-postaktiverade gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366482"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Korrigera problem med e-postleverans till e-postaktiverade gemensamma mappar

Om externa avsändare inte kan skicka meddelanden till dina e-postaktiverade gemensamma mappar och avsändarna får felet: **kunde inte hittas (550 5.4.1)** kontrollerar du att e-postdomänen är konfigurerad som en intern Relay-domän i stället för en auktoritativ domän:

1. Öppna [administrations centret för Exchange (UK)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå till **e-postflöden** \> **godkända domäner**, Välj den godkända domänen och klicka sedan på **Redigera**.

3. Om domän typen är inställd på **auktoritär**på sidan egenskaper kan du ändra värdet till **intern relä** och klicka på **Spara**.

Om externa avsändare får felet att **du inte har behörighet (550 5.7.13)** kör du följande kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) för att se behörigheterna för anonyma användare i den gemensamma mappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Om du vill tillåta externa användare att skicka e-post till den här gemensamma mappen lägger du till åtkomsten CreateItems till användaren anonym. Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
