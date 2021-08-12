---
title: Felsöka OneDrive kraschar
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921025"
---
# <a name="troubleshoot-onedrive-crashes"></a>Felsöka OneDrive kraschar

Om OneDrive kraschar flera gånger kan du prova följande felsökningssteg:

**Kontrollera att registernycklar inte har angetts:**

1. Med Registereditorn går du till HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Om DisableFileSyncNGSC finns och är inställd på 1 öppnar du nyckeln och ändrar värdet till 0.
3. Starta manuellt OneDrive genom att gå till Start ![Tryck på Windows tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i sökrutan och klicka sedan på OneDrive skrivbordsappen.

**Återställa OneDrive:**

Kommentarer:

- Om du OneDrive bort alla befintliga synkroniseringsanslutningar (inklusive ditt personliga OneDrive om det är konfigurerat).
- Du förlorar inga filer eller data om du återställer OneDrive på datorn.

**Så här återställer du OneDrive:**

1. Öppna en dialogruta genom att trycka Windows tangenten och R.
2. Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset och tryck på OK. Ett kommandofönster kan visas kort.
3. Starta manuellt OneDrive genom att gå till Start ![Tryck på Windows tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i sökrutan och klicka sedan på OneDrive skrivbordsappen.

Kommentarer:

- Om du har valt att bara synkronisera vissa mappar före återställningen måste du göra det igen när synkroniseringen är klar. Mer [information finns OneDrive vilka mappar som ska synkroniseras](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)på   datorn.
- Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.