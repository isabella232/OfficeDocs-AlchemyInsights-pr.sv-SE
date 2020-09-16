---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664188"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Alla nätverk bör vidtas för att undvika identitets problem:

1. Använd Office 365-identitet efter att ha etablerat Microsoft 365-konton för användare i Azure AD för att säkerställa att alla användare loggar in med sitt primära Microsoft-365-konto. Mer information finns i [använda Office 365-identitet för Yammer-användare](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidera flera Yammer-nätverk. Tidigare Yammer-konfigurationer gör att flera Yammer-nätverk kan anslutas till en klient organisation. Mer information finns i [klientmigrering: konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan också använda licensiering för Yammer för att blockera användare från Yammer om de inte har en licens. Mer information finns i [hantera användar licenser för Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Granska slutligen användar listan för äldre Yammer-nätverk och gör uppehåll för äldre användare. Vi rekommenderar att du inaktiverar (inaktiverar) användare i stället för att ta bort dem, eftersom borttagningen inte kan ångras. Mer information finns i [Granska Yammer-användare i nätverk anslutna till Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) och [ta bort användare](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Genom att konfigurera Yammer med de här stegen kan du också konfigurera Yammer-nätverket för eget läge för Microsoft 365. Mer information finns i [Konfigurera ditt Yammer-nätverk för eget läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).