---
title: Lösenords tillbakaskrivning fungerar inte
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243524"
---
# <a name="password-writeback-is-not-working"></a>Lösenords tillbakaskrivning fungerar inte

**Jag har problem med att konfigurera tillbakaskrivning av lösenord**

- Tillbakaskrivning av lösenord är en premium-funktion.
- Se till att du förstår licenskraven:
  - Du måste ha minst en tilldelad licens i organisationen
  - **Endast användare i molnet** – betald Office 365-SKU (O365) eller Azure AD Basic
  - **Molnanvändare och/eller** lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Mer information om licenskrav finns i [Licenskrav för självbetjäning för lösenordsåterställning i Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Du har minst ett administratörskonto och ett testanvändarkonto med en av rätt licens.
- Du måste ansluta Azure AD Connect till den primära domänkontrollant emulatorn för att lösenord ska kunna återställas. Du kan konfigurera Azure AD Connect för användning av  en primär domänkontrollant genom att högerklicka på egenskaperna för Active Directory-synkroniseringskopplingen och sedan välja **konfigurera katalogpartitioner.** Där kan du titta efter avsnittet **om anslutningsinställningar för domänkontrollanter** och markera kryssrutan som endast **heter använd önskade domänkontrollanter.**
  > [!NOTE]
  > Om det önskade DC:et inte är en PDC-emulator, kommer Azure AD Connect fortfarande att kontakta PDC för att få tillbaka lösenordet.
- Återställning av lösenord har konfigurerats och aktiverats i klientorganisationen. Mer information finns i Aktivera [att användare återställer sina Azure AD-lösenord.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Kontrollera att administratörskontot som används för att aktivera Lösenords tillbakaskrivning är ett molnadministratörskonto (som skapats i Azure AD, inte lokalt AD)
- Du har en lokal distribution av en ad eller flera skogar som kör Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de senaste service packen installerade
- Du har Azure AD Connect-verktyget installerat och förberett AD-miljön för synkronisering med molnet. Innan du testar tillbakaskrivning av lösenord ska du först slutföra en fullständig import och fullständig synkronisering från både AD och Azure AD i Azure AD Connect.
- Mer information finns i hur du gör en [fullständig synkronisering och fullständig import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jag har problem med anslutning för återskrivning av lösenord**

1. Ladda ned och aktivera den senaste versionen av [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Brandväggskonfiguration: Verktyget Azure AD Connect (1.1.443 och högre) behöver **utgående HTTPS-åtkomst** till:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillåt att inaktiva anslutningar bevaras i minst 2–3 minuter

**Jag har fortfarande problem med tillbakaskrivning av lösenord**

- Om du fortfarande har problem kan du prova att inaktivera och återaktivera tjänsten för återställning av lösenord i Azure AD Connect-verktyget
- Mer information finns i hur du [inaktiverar och återaktiverar lösenords tillbakaskrivning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
