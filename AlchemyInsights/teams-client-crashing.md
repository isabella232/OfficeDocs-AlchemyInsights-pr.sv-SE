---
title: Kraschar Teams-klienten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030670"
---
# <a name="teams-client-crashing"></a>Kraschar Teams-klienten?

Om Teams-klienten kraschar kan du prova följande:

- Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontrollera att alla [Office 365-webbadresser och adressintervall](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.

- Logga in med ditt administratörskonto och kontrollera att det inte finns några avbrott eller prestandaförsämringar i [Instrumentpanel för tjänststatus](https://docs.microsoft.com/office365/enterprise/view-service-health).

 - Som ett sista steg kan du prova att rensa Teams-klientens cache:

    1.  Avsluta Microsoft Teams-skrivbordsklienten helt. Du kan högerklicka på **Teams** i ikonfältet och klicka på **Avsluta** eller köra aktivitetshanteraren och avsluta processen helt.

    2.  Gå till Utforskaren och skriv %appdata%\Microsoft\teams.

    3.  I katalogen ser du några av följande mappar:

         - I **Programcache** går du till cachen och tar bort alla filer från cacheplatsen: %appdata%\Microsoft\teams\application cache\cache.

        - I **Blob_storage** tar du bort alla filer: %appdata%\Microsoft\teams\blob_storage.

        - I **Cache** tar du bort alla filer: %appdata%\Microsoft\teams\Cache.

        - I **databaser** tar du bort alla filer: %appdata%\Microsoft\teams\databases.

        - I **GPUCache** tar du bort alla filer: %appdata%\Microsoft\teams\GPUcache.

        - I **IndexedDB** tar du bort .db-filen: %appdata%\Microsoft\teams\IndexedDB.

        - I **Lokal lagring** tar du bort alla filer: %appdata%\Microsoft\teams\Local storage.

        - Till sist tar du bort alla filer i **tmp**: %appdata%\Microsoft\teams\tmp.

    4. Starta om Teams-klienten.
