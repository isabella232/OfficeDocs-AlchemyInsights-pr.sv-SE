---
title: 305 öka storleken på arkivpostlådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36661818"
---
# <a name="increase-the-archive-mailbox-size"></a>Öka storleken på arkivpostlådan

Office 365 [begränsar](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) storleken på arkivpostlådor baserat på licensen som är tilldelad till användarkontot. När arkivpostlådan når 90% av dess tillåtna storlek, får användaren ett e-postmeddelande. När en arkivpostlåda når sin storleksgräns kan användaren inte flytta fler objekt till arkivpostlådan. Office 365 ökar inte storleken på en arkivpostlåda när storleksgränsen har uppnåtts. I stället kan användare vidta följande åtgärder för att frigöra utrymme i arkivpostlådan:

- Exportera objekten till en PST-fil med Outlook.

- Ta bort objekt från arkivpostlådan.

Office 365 ger **obegränsad arkivering** för Office 365 Enterprise E3-och E5-licenser. En administratör måste aktivera den här funktionen innan arkivpostlådan når sin maximala storlek. När obegränsad arkivering har aktiverats kan det ta upp till 30 dagar innan ledigt utrymme läggs till i arkivpostlådan. Därför rekommenderar vi att administratörer verifierar det lediga utrymmet i arkivpostlådan, vilket gör att användaren kan fortsätta att använda arkivpostlådan när den expanderar. Mer information finns [i Översikt över obegränsad arkivering i office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) och [Aktivera obegränsad arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Mer information om hur du öppnar arkivpostlådan från Outlook finns [i Outlook-krav för åtkomst till objekt i ett automatiskt expanderat Arkiv](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Om du vill konfigurera en bevarandeprincip som automatiskt flyttar objekt till arkivpostlådan, se [Konfigurera en Arkiv-och Borttagningsprincip för postlådor i Office 365-organisationen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**** Automatisk expandering av Arkiv stöds inte för primära postlådor på Exchange 2010.
