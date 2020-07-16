---
title: Felsöka problem med inläsning av bilder i Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148300"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Felsöka problem med inläsning av bilder i Yammer

När det uppstår problem med foton och förhandsgranskningar av filer i Yammer felsöker du genom att kontrollera om problemet uppstår för alla användare, om det uppstår på mobila enheter och om det kan reproduceras när den bifogade filen laddas upp.  

**Problem med profilfoto**  

Om slutanvändare loggar in på Yammer via Microsoft 365 måste de ändra sin profil, inklusive sitt profilfoto. Om användare inte har rätt att göra profiluppdateringar kan en administratör göra uppdateringen för användaren. Mer information finns i [Visa och uppdatera din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Information om profilredigering, inklusive profilfoton, finns i [Ändra min Yammer-profil och mina inställningar](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Uppdaterade profilfoton synkroniseras på ett annat sätt än profilattribut. Användare måste logga in för att initiera en synkronisering av deras profilfoto. Mer information finns i [användarprofilbilder som uppdaterats från Office 365 till Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Information om användarlivscykeln för Yammer finns i [Hantera Yammer-användare under hela livscykeln från Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Mer information om hur synkronisering av profilbilder fungerar i Microsoft 365 finns [i Information om synkronisering av profilbilder i Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Dokumentförhandsgranskningar och problem med miniatyrbilden**  

När filer eller bilder publiceras i Yammer kanske förhandsgranskningar inte visas på grund av: 

- Filen är skadad och kan inte bearbetas.
- Filen har inte nyligen överförts till SharePoint Online, eller Yammer har ogiltiga metadata av andra skäl.
- Webbadresser som krävs för att läsa in förhandsgranskningsbilderna blockeras.
- Förhandsgranskningen av filen togs bort av användaren innan den bokfördes.
- Ett serviceproblem förhindrade att en förhandsgranskning genererades.

**Anm.)** Förhandsgranskningar för länkar och filuppladdningar kan bete sig annorlunda. Länkar till filer på internet eller länkar som kräver ytterligare autentisering kanske inte visas korrekt.

Mer information finns i [Bifoga en fil eller bild i ett Yammer-meddelande](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 