---
title: Teams-tillägg för Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629939"
---
# <a name="teams-add-in-for-mac"></a>Teams-tillägg för Mac

Följ de här anvisningarna om du vill felsöka ett tilläggsprogram för Mac-operativsystem för användare med ett team som saknas:

**Steg 1:** Om du har hybrid Exchange lokalt (2016 CU3 eller senare krävs) kan du använda Test-HMA.ps1 verktyget för att bekräfta att hybrid modern verifikation är korrekt konfigurerad. Mer information finns i [validera hybrid modern konfiguration för Outlook för iOS och Android](https://aka.ms/AA980zq).  

**Obs!** Använda UPN-adress format (till exempel [username@contoso.com](mailto:username@contoso.com)), inte domain\username. Gör detta även för användare med Exchange Online-postlådor.

**Steg 2:** Få användaren att gå till **verktyg**  >  **konton**... Leta upp och Välj kontot i Outlook för Mac. Bekräfta att username visas i UPN-format (till exempel [username@contoso.com](mailto:username@contoso.com)).

**Steg 3:** Bekräfta att användaren är en licensierad Microsoft Teams-användare. Användaren måste använda Office 365 för Mac-prenumerationen, produkt version 16,24 eller senare.