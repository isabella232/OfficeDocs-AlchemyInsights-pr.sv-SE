---
title: Teams-tillägg för Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670346"
---
# <a name="teams-add-in-for-mac"></a>Teams-tillägg för Mac

Följ de här anvisningarna om du vill felsöka ett tilläggsprogram för Mac-operativsystem för användare med ett team som saknas:

**Steg 1:** Om du har hybrid Exchange lokalt (2016 CU3 eller senare krävs) kan du använda Test-HMA.ps1 verktyget för att bekräfta att hybrid modern verifikation är korrekt konfigurerad. Mer information finns i [validera hybrid modern konfiguration för Outlook för iOS och Android](https://aka.ms/AA980zq).  

**Obs!** Använda UPN-adress format (till exempel [username@contoso.com](mailto:username@contoso.com)), inte domain\username. Gör detta även för användare med Exchange Online-postlådor.

**Steg 2:** Få användaren att gå till **verktyg**  >  **konton**... Leta upp och Välj kontot i Outlook för Mac. Bekräfta att username visas i UPN-format (till exempel [username@contoso.com](mailto:username@contoso.com)).

**Steg 3:** Bekräfta att användaren är en licensierad Microsoft Teams-användare. Användaren måste använda Office 365 för Mac-prenumerationen, produkt version 16,24 eller senare.