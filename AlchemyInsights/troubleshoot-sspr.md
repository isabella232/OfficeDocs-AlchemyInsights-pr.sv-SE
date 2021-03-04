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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430213"
---
# <a name="troubleshoot-sspr"></a>Felsöka SSPR

**Jag har problem med att konfigurera återställning av lösenord**

- Om du är administratör och vill veta hur du aktiverar självbetjäning för återställning av lösenord kan du gå till Självstudiekurs aktivera [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)och konfigurera återställning av lösenord för din organisation. Du kanske även vill granska [licenskraven.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Du måste ha minst en tilldelad licens i organisationen.
    - **Endast molnanvändare** – Office 365-betal-SKU (O365) eller Azure AD Basic
    - **Molnanvändare och/eller** lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
- Fler frågor om självbetjäning för återställning av lösenord finns i [vanliga frågor och svar.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag får ett felmeddelande**

Läs den här artikeln för att hitta vanliga fel och deras lösningar: [Felsöka självbetjäning för återställning av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag har problem med min princip för återställning av lösenord**

- Om principen för återställning av lösenord inte fungerar som förväntat eller om du har frågor om principer för återställning av lösenord läser du den här artikeln: Lösenordsprinciper och begränsningar i [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Principer för återställning av lösenord gäller inte för administratörer. Microsoft tillämpar en stark standardprincip för återställning av lösenord med två porter för alla Azure-administratörsroller. Kontrollera att du testar med en användare som inte är administratör. Mer information om administratörsåterställningsprincipen finns i den här artikeln: Skillnader i [administratörsåterställningsprincip.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Jag vill inte att mina användare ska registrera ytterligare säkerhetsinformation för återställning av lösenord**

Du kan fylla i data i förväg (e-post- och telefonattribut) för användarna med hjälp av ett API, PowerShell eller Azure AD Connect. Så här läser du:

- [Distribuera lösenordsåterställning utan att användare måste registrera sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Vilka data används vid återställning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag vill att användarna ska registrera sin ytterligare säkerhetsinformation för återställning av lösenord**

1. Be användarna registrera sin säkerhetsinformation för återställning av självbetjäningslösenord genom att dirigera dem [till aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. När data har fyllts i för användaren (av användaren eller av administratören) dirigerar du användaren till [aka.ms/sspr](https://passwordreset.microsoftonline.com/) så att användarna kan återställa sina egna lösenord.
1. Om användarna fortfarande har problem är de troligen **synkroniserade användare med federerad** hash- eller lösenordshashar.  Det innebär att det troligtvis finns ett problem med tjänsten Password Writeback.