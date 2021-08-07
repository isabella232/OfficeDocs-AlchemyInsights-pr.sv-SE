---
title: Password Writeback fungerar inte
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999762"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback fungerar inte

**Jag har problem med att konfigurera tillbakaskrivning av lösenord**

- Återskrivning av lösenord är en premiumfunktion.
- Se till att du förstår licenskraven:
  - Du måste ha minst en licens tilldelad i din organisation
  - **Endast molnanvändare** – alla Office 365 (O365) betal-SKU eller Azure AD Basic
  - **Användare i molnet och/eller** lokalt – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Mer information om licenskrav finns i [Licenskrav för självbetjäning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) för självbetjäning för Azure AD
- Du har minst ett administratörskonto och ett testanvändarkonto med en av rätt licens.
- Du måste ansluta Azure AD-Anslut till den primära domänkontrollanten för Emulator för att lösenordsskrivning ska fungera. Du kan konfigurera Azure AD Anslut att använda en primär  domänkontrollant genom att högerklicka på egenskaperna för Active Directory-synkroniseringskopplingen och sedan välja konfigurera **katalogpartitioner**. Leta därifrån efter **domänkontrollantens anslutningsinställningar och** markera kryssrutan använd endast **önskade domänkontrollanter**.
  > [!NOTE]
  > Om den önskade DC:n inte är en PDC-emulator, kommer Azure AD Anslut fortfarande att kontakta PDC:n för tillbakaskrivning av lösenord.
- Återställning av lösenord har konfigurerats och aktiverats i klientorganisationen. Mer information finns i Aktivera [så att användare kan återställa sina Azure AD-lösenord.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Kontrollera att det administratörskonto som används för att aktivera Lösenords tillbakaskrivning är ett molnadministratörskonto (skapas i Azure AD inte lokalt AD)
- Du har en lokal distribution med en ad eller flera skogar som kör Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de senaste service packen installerade
- Du har Azure AD Anslut installerat och du har förberett AD-miljön för synkronisering till molnet. Innan du testar tillbakaskrivning av lösenord ska du först slutföra en fullständig import och fullständig synkronisering från både AD och Azure AD i Azure AD Anslut.
- Mer information finns i hur du gör en fullständig [synkronisering och fullständig import i Azure AD Anslut](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jag har problem med återskrivning av lösenord**

1. Ladda ned och aktivera den senaste versionen av [Azure AD Anslut](https://www.microsoft.com/download/details.aspx?id=47594)
2. Brandväggskonfiguration: Verktyget Azure AD Anslut (1.1.443 och högre) behöver **utgående HTTPS-åtkomst** till:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillåt att inaktiva anslutningar finns kvar i minst 2–3 minuter

**Jag har fortfarande problem med tillbakaskrivning av lösenord**

- Om du fortfarande har problem kan du prova att inaktivera och återaktivera tjänsten för tillbakaskrivning av lösenord i Azure AD Anslut verktyget
- Mer information finns i inaktivera och [återaktivera tillbakaskrivning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
