---
title: Aktivera tillbakaskrivning av lösenord i Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093373"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivera tillbakaskrivning av lösenord i Azure AD Connect

Om du vill aktivera självbetjäning för återställning av tillbakaskrivning av lösenord aktiverar du först alternativet för tillbakaskrivning i Azure AD Connect. Gå igenom följande steg från Azure AD Connect-servern:

1. Logga in på Azure AD Connect-servern och starta **konfigurations guiden för Azure AD Connect** .
2. På **Välkomstsidan** klickar du på **Konfigurera**.
3. På sidan **Ytterligare tasks** klickar du på **Anpassa synkroniseringsalternativ** och sedan på **Nästa**.
4. På sidan **Anslut till Azure AD** skriver du dina globala administratörsautentiseringsuppgifter. Klicka sedan på **Nästa**.
5. På sidorna **Anslut kataloger** och **Domän-/OU-filtrering** klickar du på **Nästa**.
6. På sidan **Valfria funktioner** väljer du **Tillbakaskrivning av lösenord** och klickar på **Nästa**.
7. På sidan **Redo att konfigurera** klickar du på **Konfigurera** och väntar tills processen har slutförts.
8. När konfigurationen är klar klickar du på **Avsluta**.

Med tillbakaskrivning av lösenord aktiverat i Azure AD Connect konfigurerar du Azure AD-SSPR för tillbakaskrivning.  Om du vill aktivera tillbakaskrivning av lösen ord i SSPR gör du så här:

1. Logga in på Azure-portalen med ditt globala administratörskonto.
2. Sök efter och välj **Azure Active Directory**, klicka på **Återställ lösenord** och klicka sedan på **Lokal integration**.
3. Ange alternativet för **Skriv tillbaka lösenordet till din lokala katalog?** **Ja**.
4. Ställ in alternativet för **Tillåt användare att låsa upp konton utan att återställa deras lösen ord?** **Ja**.
5. När du är klar klickar du på **Spara**.

Mer information finns i [Aktivera automatisk återställning av lösenord i Azure Active Directory – tillbakaskrivning i en lokal miljö](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  När en administratör återställer en användares lösenord i Azure-portalen, om användaren är federerad eller lösenordets-hash är synkroniserad, skrivs lösenordet tillbaka till lokalt. Denna funktionalitet kräver Azure Premium-licens (P1 eller P2) och stöds för nuvarande inte i Office administrationsportalen.
