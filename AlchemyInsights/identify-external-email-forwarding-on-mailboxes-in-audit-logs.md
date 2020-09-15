---
title: Identifiera extern vidarebefordran av e-post i post lådor i gransknings loggar
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696315"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när extern e-postvidarebefordran är konfigurerad på post lådor

När en Microsoft 365-användare konfigurerar extern e-postvidarebefordran i en post låda granskas aktiviteten som en del av cmdleten **set-post låda** . Du kan se aktiviteten med hjälp av gransknings loggs ökning i centret för säkerhets & efterlevnad.

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå till sidan **Sök**  >  **gransknings loggs sökning** .

3. Välj datum intervall i fälten **start datum** och **slutdatum** . Du behöver inte ange ett användar namn. Kontrol lera att fältet **aktiviteter** är inställt på **Visa resultat för alla aktiviteter**.

4. Klicka på **Sök**.

Klicka på **filter resultat** och skriv **in post låda** i rutan aktivitets filter. Välj en gransknings post i resultatet. I den utfällbara **informationen** klickar du på **Mer information**. Du måste granska detaljerna för varje gransknings post för att avgöra om aktiviteten är relaterad till vidarebefordran via e-post.

- **ObjectID**: Ali Aset för post lådan som har ändrats.

- **Parametrar**: _ForwardingSmtpAddress_ anger mål-e-postadress.

- **UserID**: användaren som konfigurerade e-postvidarebefordran på post lådan i fältet **ObjectID** .

Mer information finns i [bestämma vem som konfigurerar e-postvidarebefordran för en post låda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
