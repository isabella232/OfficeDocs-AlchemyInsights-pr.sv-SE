---
title: Felsöka OneDrive-krascher
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826217"
---
# <a name="troubleshoot-onedrive-crashes"></a>Felsöka OneDrive-krascher

Om OneDrive kraschar upprepade gånger kan du prova följande felsökningssteg:

**Kontrollera att registernycklar inte har angetts:**

1. Med Registereditorn går du till HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Om DisableFileSyncNGSC finns och är inställd på 1 öppnar du nyckeln och ändrar värdet till 0.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsprogrammet.

**Återställa OneDrive:**

Kommentarer:

- Om du återställer OneDrive kopplas alla befintliga synkroniseringsanslutningar bort (inklusive din personliga OneDrive om den är konfigurerad).
- Du förlorar inga filer eller data genom att återställa OneDrive på datorn.

**Återställa OneDrive:**

1. Öppna en dialogruta genom att trycka på Windows-tangenten och R.
2. Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset och tryck på OK. Ett kommandofönster kan visas kort.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsprogrammet.

Kommentarer:

- Om du har valt att bara synkronisera vissa mappar före återställningen måste du göra det igen när synkroniseringen är klar. Mer [information finns i Välja vilka OneDrive-mappar som ska synkroniseras](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)på   datorn.
- Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.