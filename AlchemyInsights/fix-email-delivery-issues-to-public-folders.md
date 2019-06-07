---
title: Åtgärda problem med e-post levereras till e-postfunktioner gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752698"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Åtgärda problem med e-post levereras till e-postfunktioner gemensamma mappar

Om externa avsändare kan inte skicka meddelanden till din e-postfunktioner gemensamma mappar och avsändare visas fel: **kunde inte hittas (550 5.4.1)**, verifiera e-domänen för den gemensamma mappen konfigureras som en intern relay domän i stället för en auktoritär domän:

1. Öppna [Exchange administratörscenter (UK)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå till **e-postflödet** \> **accepterade domäner**, markera accepterade domänen och klicka sedan på **Redigera**.

3. I egenskaperna för sidan som öppnas om typen domän är **auktoritära**, ändra värdet till **interna relay** och klicka på **Spara**.

Om externa avsändare får fel **du inte har behörighet (550 5.7.13)**, kör du följande kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) Se behörigheter för anonyma användare i den delade mappen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Tillåt externa användare att skicka e-post till mappen genom att lägga till CreateItems access rätt till användaren Anonym. Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
