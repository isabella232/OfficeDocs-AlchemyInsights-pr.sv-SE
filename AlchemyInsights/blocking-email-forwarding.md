---
title: 726 blockerar e-postvidarebefordran
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219873"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blockera eller avblockera e-postvidarekoppling

Information om hur du aktiverar och inaktiverar e-postvidarekoppling för en viss post låda finns i [Konfigurera e-postvidarekoppling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

På klient organisations nivå sker kontrollen av extern vidarebefordring med principen för utgående anti-spam. Om den är inaktive rad eller automatisk kan det vara en snabb överföring av e-post med fel meddelandet "550 5.7.520 åtkomst nekad". Om vidarebefordran har ställts in på att blockeras är det fel som användarna ser.

Om vidarebefordran blockeras bör du kontrol lera att den är konfigurerad för att aktivera extern vidarebefordring. Du kan kontrol lera filtrerings principen för utgående e-post från säkerhets-och kompatibilitetstillstånd eller genom att köra kommandona GET-HostedOutboundSpamFilterPolicy | fl-namn, AutoForwardingMode. Om du vill ställa in blockering av autoforwarding visar kommandot samma tillstånd.

Obs! Du bör behålla den externa autoforwarden inaktive rad i standard filtrerings filtret för utgående e-post och bara aktivera den för användare som behöver extern vidarebefordran genom att skapa en egen princip för dessa användare. Du kan läsa mer om hur du [konfigurerar extern vidarebefordran av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).