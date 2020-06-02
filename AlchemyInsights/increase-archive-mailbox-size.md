---
title: 305 Öka storleken på arkivbrevlådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508826"
---
# <a name="increase-the-archive-mailbox-size"></a>Öka storleken på arkivpostlådan

Microsoft 365 [begränsar](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) storleken på arkivpostlådor baserat på den licens som har tilldelats användarkontot. När arkivpostlådan når 90 % av den tillåtna storleken får användaren ett e-postmeddelande. När en arkivpostlåda når sin storleksgräns kan användaren inte flytta fler objekt till arkivpostlådan. Microsoft 365 ökar inte storleken på en arkivpostlåda när storleksgränsen har uppnåtts. I stället kan användarna vidta följande åtgärder för att frigöra utrymme i arkivpostlådan:

- Exportera objekten till en PST-fil med Outlook.

- Ta bort objekt från arkivpostlådan.

Microsoft 365 tillhandahåller **obegränsad arkivering** för Office 365 Enterprise E3- och E5-licenser. En administratör måste aktivera den här funktionen innan arkivpostlådan når sin maximala storlek. När obegränsad arkivering är aktiverat kan det ta upp till 30 dagar innan ledigt utrymme läggs till i arkivbrevlådan. Därför rekommenderar vi att administratörer verifierar det lediga utrymmet i arkivpostlådan, vilket gör att användaren kan fortsätta använda arkivpostlådan medan den expanderar. Mer information finns [i Översikt över obegränsad arkivering i Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) och Aktivera obegränsad arkivering i Microsoft [365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Mer information om hur du kommer åt arkivpostlådan från Outlook finns i [Outlook-krav för åtkomst till objekt i ett automatiskt expanderat arkiv](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Information om hur du konfigurerar en bevarandeprincip som automatiskt flyttar objekt till arkivpostlådan finns i [Konfigurera en arkiv- och borttagningsprincip för postlådor i microsoft 365-organisationen](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Automatisk**expanderande arkiv stöds inte för primära postlådor i Exchange 2010.
