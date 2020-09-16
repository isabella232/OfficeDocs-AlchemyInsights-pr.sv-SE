---
title: Felsöka OneDrive-krascher
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665016"
---
# <a name="troubleshoot-onedrive-crashes"></a>Felsöka OneDrive-krascher

Om OneDrive kraschar upprepade gånger kan du försöka med följande fel söknings steg:

**Kontrol lera att register nycklar inte är inställda:**

1. Använd Registereditorn och navigera till HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Om DisableFileSyncNGSC finns och är 1 öppnar du den och ändrar värdet till 0.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i sökrutan och klicka sedan på OneDrive-programmet.

**Återställ OneDrive:**

Kommentarer:

- Om du återställer OneDrive kopplas alla befintliga synkroniseringskopplingar (inklusive ditt personliga OneDrive om det är konfigurerat).
- Du förlorar inte filer eller data genom att återställa OneDrive på datorn.

**Så här återställer du OneDrive:**

1. Öppna dialog rutan Kör genom att trycka på Windows-tangenten och R.
2. Skriv% localappdata% \Microsoft\OneDrive\onedrive.exe/reset. och klicka på OK. Ett kommando fönster kan komma att visas kort.
3. Starta OneDrive manuellt genom att gå till Start ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i sökrutan och klicka sedan på OneDrive-programmet.

Kommentarer:

- Om du inte har valt att synkronisera vissa mappar före återställningen måste du göra det när synkroniseringen är klar. Läsa [Välj vilka OneDrive-mappar som ska synkroniseras med din dator](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   för mer information.
- Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.