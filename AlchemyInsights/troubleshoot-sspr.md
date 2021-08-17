---
title: Felsöka SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038976"
---
# <a name="troubleshoot-sspr"></a>Felsöka SSPR

**Jag har problem med att konfigurera återställning av lösenord**

- Om du är administratör och vill veta hur du aktiverar självbetjäning för återställning av lösenord kan du gå till Självstudiekurs aktivera [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), och konfigurera återställning av lösenord för din organisation. Du kanske även vill granska [licenskraven.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Du måste ha minst en licens tilldelad i organisationen.
    - **Endast molnanvändare** – alla Office 365 (O365) betal-SKU eller Azure AD Basic
    - **Användare i molnet och/eller** lokalt – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
- Fler frågor om självbetjäning för återställning av lösenord finns i [Vanliga frågor och svar.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag får ett felmeddelande**

Läs den här artikeln om du vill hitta vanliga fel och deras lösningar: [Felsöka lösenordsåterställning via självbetjäning](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag har problem med min princip för återställning av lösenord**

- Om principen för återställning av lösenord inte fungerar som förväntat eller om du har frågor om principer för återställning av lösenord läser du den här artikeln: Lösenordsprinciper och begränsningar [i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Principerna för återställning av lösenord gäller inte för administratörer. Microsoft tillämpar en stark standardprincip med två grindar för återställning av lösenord för alla Azure-administratörsroller. Kontrollera att du testar med en användare som inte är administratör. Mer information om administratörsåterställningsprincipen finns i den här artikeln: Skillnader [i administratörsåterställningsprincip.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Jag vill inte att mina användare ska registrera ytterligare säkerhetsinformation för återställning av lösenord**

Du kan fylla i data (e-post- och telefonattribut) för dina användare i förväg med hjälp av ett API, PowerShell eller Azure AD Anslut. Så här läser du:

- [Distribuera lösenordsåterställning utan att användare måste registrera sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Vilka data används vid återställning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag vill att användarna ska registrera sin ytterligare säkerhetsinformation för återställning av lösenord**

1. Be användarna registrera sin säkerhetsinformation för återställning av självbetjäning för lösenord genom att hänvisa dem [till aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. När data har fyllts i för användaren (av användaren eller administratören) dirigerar du användaren [till aka.ms/sspr](https://passwordreset.microsoftonline.com/) så att användarna kan återställa sina egna lösenord.
1. Om användarna fortfarande har problem är de troligen **synkroniserade användare med** hash- **eller federerade** lösenord. Det innebär att det troligtvis är problem med tjänsten Password Writeback.