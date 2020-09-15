---
title: Felsöka Lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664944"
---
# <a name="troubleshoot-password-synchronization"></a>Felsöka Lösenordssynkronisering

För att felsöka problem med Lösenordssynkronisering kan du börja använda denna åtgärd för att ansluta till AAD för att avgöra varför lösen ord inte synkroniseras. Börja genom att gå till [Hantera direkt synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Öppna en ny Windows PowerShell-session på din Azure AD Connect-Server och välj alternativet **Kör som administratör** .

2. Kör Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy unrestricted.

3. Starta Azure AD Connect-guiden.

4. Gå till sidan Ytterligare aktiviteter > **Felsöka**  >  **Nästa**.

5. Välj **Starta** för att öppna fel söknings menyn i PowerShell.

6. Välj **Felsök Lösenordssynkronisering**.

    Problemet är vanligt vis att ett lösen ord inte är synkroniserat för ett visst användar konto.

    **Anteckningar** Det går inte att synkronisera lösen ord om den senaste lyckade lösen ords synkroniseringen var för lite sedan.

Mer hjälp med att felsöka Lösenordssynkronisering finns i [Felsöka lösen ord för Lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).