---
title: 305 öka Arkivera postlådans storlek
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391569"
---
# <a name="increase-the-archive-mailbox-size"></a>Öka Arkivera postlådans storlek

Office 365 [gränser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) storleken på arkivet postlådor baserat på den licens som tilldelats användarkontot. När arkivet postlåda når 90% av den tillåtna storleken, får användaren ett e-postmeddelande. När en Arkivera postlåda uppnår storleksgränsen, kan inte användaren flytta flera objekt till arkivet postlåda. Office 365 kommer inte att öka storleken på en Arkivera postlåda när gränsen har nåtts. Användare kan i stället vidta följande åtgärder för att frigöra utrymme i postlådan arkivera:

- Exportera de objekt till en PST-fil i Outlook

- Ta bort objekt från postlådan arkivera.

Office 365 ger **obegränsad arkivering** för licenser för Office 365 Enterprise E3 och E5. En administratör måste aktivera funktionen innan Arkivera postlåda når sin maximala storlek. Det kan ta upp till 30 dagar innan ledigt utrymme läggs till arkivet postlåda när obegränsat arkivering aktiveras. Därför rekommenderar vi att administratörer kontrollera ledigt utrymme i arkivet postlådan, som gör att användaren kan fortsätta att använda Arkivera postlåda medan den expanderas. Mer information finns i [Översikt över obegränsad arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) och [Aktivera obegränsad arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Mer information om åtkomst till Arkiv-postlåda i Outlook finns i [Outlook krav för åtkomst till objekt i ett Arkiv expanderas automatiskt](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Om du vill konfigurera en bevarandeprincip som automatiskt flyttar objekt till arkivet postlåda finns i [Konfigurera en arkivera och ta bort princip för postlådor i Office 365-organisation](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Anmärkning**: Arkiv utökas automatiskt stöds inte för primära postlådor i Exchange 2010.
