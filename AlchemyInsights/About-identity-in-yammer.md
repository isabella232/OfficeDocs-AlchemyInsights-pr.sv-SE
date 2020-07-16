---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148301"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Vi rekommenderar att alla nätverk vidtar följande åtgärder för att undvika identitetsrelaterade problem:

1. Framtvinga Office 365-identitet efter etablering av Microsoft 365-konton för användare i Azure AD för att säkerställa att alla användare loggar in med sitt primära Microsoft 365-konto. Mer information finns i [Framtvinga Office 365-identitet för Yammer-användare](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidera flera Yammer-nätverk. Äldre Yammer-konfigurationer gör det möjligt för flera Yammer-nätverk att anslutas till en klient. Mer information finns i [Nätverksmigrering - Konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan också tillämpa licensiering för Yammer för att blockera användare från Yammer om de inte har en licens. Mer information finns [i Hantera Yammer-användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Slutligen granska användarlistan för äldre Yammer-nätverk och pausa äldre användare. Vi rekommenderar att du pausar (inaktiverar) användare i stället för att ta bort dem, eftersom borttagningen är oåterkallelig. Mer information finns [i Granska Yammer-användare i nätverk som är anslutna till Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) och [Ta bort användare](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Genom att konfigurera Yammer med hjälp av dessa steg är du också redo att konfigurera Yammer-nätverket för inbyggt läge för Microsoft 365. Mer information finns i [Konfigurera Yammer-nätverket för inbyggt läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).