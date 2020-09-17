---
title: 305 öka storleken på Arkiv post lådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778601"
---
# <a name="increase-the-archive-mailbox-size"></a>Öka storleken på Arkiv post lådan


Om du vill att vi ska köra automatisk kontroll för de inställningar som nämns nedan, väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för den användare som behöver Arkiv post lådans storlek.

Microsoft 365 [begränsar](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) storleken på Arkiv post lådor som baseras på den licens som har tilldelats till användar kontot. När Arkiv post lådan når 90% av dess tillåtna storlek får användaren ett e-postmeddelande. När en Arkiv post låda når sin storleks gräns kan användaren inte flytta fler objekt till Arkiv post lådan. Microsoft 365 ökar inte storleken på en Arkiv post låda när storleks gränsen är nådd. I stället kan användarna vidta följande åtgärder för att frigöra utrymme i Arkiv post lådan:

- Exportera objekten till en PST-fil med hjälp av Outlook.

- Ta bort objekt från Arkiv post lådan.

Microsoft 365 tillhandahåller **obegränsad arkivering** för Office 365 Enterprise E3-och E5-licenser. En administratör måste aktivera den här funktionen innan Arkiv post lådan når maximal storlek. När obegränsad arkivering är aktive rad kan det ta upp till 30 dagar innan ledigt utrymme läggs till i Arkiv post lådan. Därför rekommenderar vi att administratörer verifierar det lediga utrymmet i Arkiv post lådan, vilket gör det möjligt för användaren att fortsätta använda Arkiv post lådan medan den expanderas. Mer information finns i [Översikt över obegränsad arkivering i microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) och [Aktivera obegränsad arkivering i Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Mer information om hur du öppnar Arkiv post lådan från Outlook finns i artikeln [om att få åtkomst till objekt i ett automatiskt expanderat Arkiv](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Om du vill konfigurera en bevarande princip som automatiskt flyttar objekt till Arkiv post lådan läser du konfigurera [en princip för arkivering och borttagning för post lådor i din Microsoft 365-organisation](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Obs!** det går inte att extrahera arkiv automatiskt för primära post lådor i Exchange 2010.
