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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918955"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Vi rekommenderar att alla nätverk gör följande för att undvika identitetsrelaterade problem:

1. Tillämpa Office 365-identitet efter etablering Microsoft 365-konton för användare i Azure AD för att säkerställa att alla användare loggar in med sitt primära Microsoft 365 konto. Mer information finns i Tillämpa [Office 365 identitet för Yammer användare.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Konsolidera flera Yammer nätverk. Med Yammer konfigurationer kan flera Yammer anslutas till en klientorganisation. Mer information finns i [Nätverksmigrering – Konsolidera flera Yammer nätverk.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Du kan också tillämpa licensiering för Yammer att blockera användare från Yammer om de inte har en licens. Mer information finns i [Hantera Yammer användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Granska slutligen användarlistan för äldre användare Yammer och inaktivera äldre användare. Vi rekommenderar att du inaktiverar (inaktiverar) användare i stället för att ta bort dem, eftersom borttagningen är bestående. Mer information finns i Granska [granskning av Yammer i nätverk anslutna till Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) och Ta bort [användare.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Genom att Yammer med hjälp av de här stegen är du också redo att konfigurera Yammer-nätverket för inbyggt läge för Microsoft 365. Mer information finns i [Konfigurera ditt Yammer för inbyggt läge för Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)