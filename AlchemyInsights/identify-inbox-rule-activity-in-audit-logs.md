---
title: Identifiera Inkorgen regeln aktivitet i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539191"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifiera Inkorgen regeln aktivitet i granskningsloggar

Du kan använda Granska loggen Sök i Office 365 säkerhet & regelefterlevnadscentret Inkorgen regeln händelser (skapa, ändra och ta bort regler för Inkorgen).

1. Logga in på [Office 365 säkerhet & regelefterlevnadscentret](https://protection.office.com/).

2. Gå till **Sök** > **Granska loggen** söksida.

3. Välj datumintervall i fälten **startdatum** och **slutdatum** .

4. Under **Aktiviteter för Exchange-postlåda**, Kontrollera fältet **aktiviteter** anges till **New-InboxRule skapa/ändra/aktivera/inaktivera Inkorgsregel**.

5. Klicka på **Sök**.

Markera en granskningspost i resultatet. Klicka på **Mer Information**i information-utfällbar. Information om inställningar för Inkorgen regeln visas i fältet **parametrar** .

Mer information finns i [fastställa om en användare har skapat en Inkorgsregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
