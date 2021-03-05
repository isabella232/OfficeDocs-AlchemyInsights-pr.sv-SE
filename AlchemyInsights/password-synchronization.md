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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483085"
---
# <a name="password-synchronization"></a>Lösenordssynkronisering

**Synkronisering av lösenordshashar fungerar inte alls**

Några vanliga problem som kunder stöter på när synkronisering av lösenordshashar inte fungerar är:

- Det Active Directory-konto som används av Azure AD Connect  för att  kommunicera med lokalt Active Directory beviljas inte behörigheten Replikera katalogändringar och Replikera katalogändringar alla, vilket krävs för lösenordssynkronisering – Du måste åtgärda detta genom att tilldela behörigheterna till Active Directory-kontot.
- Synkronisering av lösenordshashar inaktiveras när en  administratör har ändrat User Sign-In-metoden från lösenordssynkronisering till ett annat alternativ,  till exempel Federation med **AD FS** i Azure AD Connect-guiden – Du kan åtgärda det genom att aktivera synkroniseringsfunktionen för lösenordshashar på nytt i guiden Azure AD Connect.
- Anslutningsproblem med lokal Active Directory. Vissa domänkontrollanter kan till exempel inte nås av [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect, eller så blockeras de portar som krävs av brandväggen – Du måste åtgärda detta genom att säkerställa att anslutningen mellan Azure AD Connect-servern och den lokala Active Directory fungerar som den ska.
- Azure AD Connect-servern är för närvarande i mellanlagringsläge, vilket gör att servern inte kan [lösenordshashar](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)- För att felsöka problemet följer du stegen som beskrivs i avsnittet Felsöka lösenordssynkronisering med Azure AD Connect-synkronisering – Inga lösenord synkroniseras.

**Synkronisering av lösenordshashar fungerar inte för vissa av mina användare**

1. Om du lade märke till att lösenordshashar  inte synkroniseras för en användare kan du använda felsökningsaktiviteten i Azure AD Connect för att undersöka och lösa problemet. Utför följande uppgifter:

    a. [Köra felsökningsaktiviteten i guiden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Använd cmdleten för felsökning för att undersöka problemet med synkronisering av lösenordshashar för en viss användning](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokala Active Directory-användarobjektet är aktiverat för **användaren måste ändra lösenord vid nästa inloggningsalternativ.** När det här alternativet är aktiverat tilldelas användaren ett tillfälligt lösenord och uppmanas att ändra lösenordet vid nästa inloggning. Azure AD Connect synkroniserar inte tillfälliga lösenord med Azure AD.

Lös problemet genom att utföra någon av följande uppgifter:

- Be användaren att logga in på det lokala programmet (till exempel Windows-skrivbordet) och ändra lösenordet. Det nya lösenordet synkroniseras till Azure AD.
- Be en administratör uppdatera användarens lösenord utan att aktivera alternativet Användaren måste ändra lösenordet vid nästa inloggning och dela det nya lösenordet med användaren.

3. Det lokala Active Directory-användarobjektet är inte **korrekt konfigurerat för objektsynkronisering** eller lösenordssynkronisering. För att felsöka det här problemet följer du stegen som beskrivs i Felsöka synkronisering [av lösenordshashar med Azure AD Connect-synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







