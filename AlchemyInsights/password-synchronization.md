---
title: Lösenordssynkronisering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960853"
---
# <a name="password-synchronization"></a>Lösenordssynkronisering

**Synkronisering av lösenordshashar fungerar inte alls**

Några vanliga problem som kunder stöter på när synkronisering av lösenordshashar inte fungerar är:

- Det Active Directory-konto som används av Azure AD Anslut för  att kommunicera  med lokal Active Directory beviljas inte behörigheten Replikera katalogändringar och Replikera katalogändringar alla, vilket krävs för lösenordssynkronisering – Du måste åtgärda detta genom att tilldela behörigheterna till Active Directory-kontot.
- Synkronisering av lösenordshashar inaktiveras när en administratör  har ändrat User Sign-In-metoden från Lösenordssynkronisering till ett annat alternativ, till exempel  Federation med **AD FS** i Azure AD Anslut-guiden – Du kan åtgärda det genom att aktivera synkroniseringen av lösenordshashar igen i Azure AD Anslut-guiden.
- Anslutningsproblem med lokal Active Directory. Vissa domänkontrollanter kan till exempel inte nås av Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD Anslut eller så blockeras de portar som krävs av brandväggen – Du måste åtgärda detta genom att säkerställa att anslutningen mellan Azure AD Anslut-servern och den lokala Active Directory fungerar korrekt.
- Azure AD Anslut-servern för närvarande i mellanlagringsläge. Det leder till att servern inte kan [lösenordshashar](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)– Felsöka problemet genom att följa stegen som beskrivs i avsnittet Felsöka lösenordssynkronisering med Azure AD Anslut-synkronisering – Inga lösenord synkroniseras.

**Synkronisering av lösenordshashar fungerar inte för vissa av mina användare**

1. Om du lade märke till att lösenordshashar  inte synkroniseras för en användare kan du använda felsökningsaktiviteten i Azure AD Anslut undersöka och lösa problemet. Utför följande uppgifter:

    a. [Köra felsökningsaktiviteten i guiden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Använd cmdleten för felsökning för att undersöka synkroniseringsproblem för lösenordshashar för en viss användning](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokala Active Directory-användarobjektet är aktiverat för **Användaren måste ändra lösenord vid nästa inloggningsalternativ.** När det här alternativet är aktiverat får användaren ett tillfälligt lösenord och uppmanas att ändra lösenordet vid nästa inloggning. Azure AD Anslut synkroniserar inte tillfälliga lösenord till Azure AD.

Lös problemet genom att utföra någon av följande åtgärder:

- Be användaren att logga in på det lokala programmet (till exempel på Windows skrivbord) och ändra lösenordet. Det nya lösenordet synkroniseras till Azure AD.
- Be en administratör uppdatera användarens lösenord utan att aktivera alternativet Användaren måste ändra lösenordet vid nästa inloggning och dela det nya lösenordet med användaren.

3. Det lokala Active Directory-användarobjektet är inte **korrekt konfigurerat för objektsynkronisering** eller lösenordssynkronisering. Om du vill felsöka problemet följer du stegen som beskrivs i Felsöka synkronisering av [lösenordshashar med Azure AD Anslut synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







