---
title: Felsökning av meddelanden om nekad åtkomst till OneDrive för företag webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957811"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsökning av meddelanden om nekad åtkomst till OneDrive för företag webbplatser

Det här problemet uppstår oftast när en användare tas bort och skapas på nytt med samma huvudnamn (UPN). Det nya kontot skapas med ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller en OneDrive har användaren ett felaktigt PUID. I ett andra scenario ingår katalogsynkronisering med en Organisationsenhet (OU) i Active Directory. Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan OU och synkroniseras om med SharePoint kan problemet uppstå.

1. Du kan lösa problemet genom att återställa det ursprungliga UPN med stegen i artikeln [Återställa en användare i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Om du inte kan återställa den ursprungliga användaren ska du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av de här stegen, Ta bort en användare från [listan med användarinformation.]() 
3. När detta är klart kan du kontrollera att användaren har administratörsrättigheter för OneDrive-webbplatsen genom att följa stegen för att Lägga till administratörer för en [användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Mer information om behörighetsnivåer finns i artikeln Förstå [behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
