---
title: Felsöka lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387895"
---
# <a name="troubleshoot-password-synchronization"></a>Felsöka lösenordssynkronisering

Om du vill felsöka problem med lösenordssynkronisering börjar du med den här felsökningsuppgiften för AAD Connect för att ta reda på varför lösenord inte synkroniseras. Börja med att gå till [Hantera direktsynkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Öppna en ny Windows PowerShell-session på din Azure AD Connect-server och välj alternativet **Kör som administratör.**

2. Kör Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Obegränsad.

3. Starta Azure AD Connect-guiden.

4. Gå till sidan Ytterligare uppgifter > **felsöka**  >  **nästa**.

5. Välj **Starta** för att öppna felsökningsmenyn för PowerShell.

6. Välj **Felsöka lösenordssynkronisering**.

    Problemet är vanligtvis att ett lösenord inte synkroniseras för ett visst användarkonto.

    **Anteckningar** Lösenordssynkronisering misslyckas om den senaste lyckades lösenordssynkroniseringen var för en tid sedan.

Mer hjälp med felsökning av lösenordssynkronisering finns i [Felsöka synkronisering av lösenordshÃ¶kning med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).