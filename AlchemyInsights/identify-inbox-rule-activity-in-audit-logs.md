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
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755055"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifiera Inkorgen regeln aktivitet i granskningsloggar

Du kan använda Granska loggen Sök i säkerhet & regelefterlevnadscentret Inkorgen regeln händelser (skapa, ändra och ta bort regler för Inkorgen).

1. Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)

2. Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.

3. Välj datumintervall i fälten **startdatum** och **slutdatum** .

4. Under **Aktiviteter för Exchange-postlåda**, Kontrollera fältet **aktiviteter** anges till **New-InboxRule skapa/ändra/aktivera/inaktivera Inkorgsregel**.

5. Klicka på **Sök**.

Markera en granskningspost i resultatet. Klicka på **Mer Information**i information-utfällbar. Information om inställningar för Inkorgen regeln visas i fältet **parametrar** .

Mer information finns i [fastställa om en användare har skapat en Inkorgsregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
