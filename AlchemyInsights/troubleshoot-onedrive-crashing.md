---
title: Felsöka OneDrive kraschar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749170"
---
# <a name="troubleshoot-onedrive-crashes"></a>Felsöka OneDrive kraschar

Om OneDrive kraschar flera gånger provar du de här felsökningsstegen:

**Kontrollera att registernycklarna inte är inställda:**

1. Använda Registereditorn och navigera till HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Om DisableFileSyncNGSC finns och är inställd på 1 öppnar du nyckeln och ändrar värdet till 0.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsappen.

**Återställa OneDrive:**

Kommentarer:

- Om du återställer OneDrive kopplas alla befintliga synkroniseringsanslutningar frånkopplad från alla dina befintliga synkroniseringsanslutningar (inklusive din personliga OneDrive om den är konfigurerad).
- Du förlorar inte filer eller data genom att återställa OneDrive på datorn.

**Så här återställer du OneDrive:**

1. Öppna dialogrutan Kör genom att trycka på Windows-tangenten och R.
2. Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset och tryck på OK. Ett kommandofönster kan visas en kort stund.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsappen.

Kommentarer:

- Om du bara hade valt att synkronisera vissa mappar före återställningen måste du göra det igen när synkroniseringen har slutförts. Läs [Välj vilka OneDrive-mappar som ska synkroniseras med datorn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)för mer   information.
- Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.