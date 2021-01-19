---
title: Felsöka användar problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901339"
---
# <a name="announcements"></a>Meddelanden

Följ Googles vägledning om testning för kompatibilitet för att testa om dina program påverkas. Googles vägledning finns i https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Kontrol lera att du använder system webvy eller system granskning när du loggar in på användare med Google-konton. Mer information finns i [problem med att logga in på program via Chrome-webbläsaren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Jag kan inte skapa en ny användare i min Azure AD-katalog**

Så här felsöker du problemet med att skapa en ny användare i Azure AD:

1. Se till att du har behörighet att skapa en ny standard användare. Det är bara rollen global administratör eller användar administratör i Azure Active Directory (AD) som kan skapa en ny standard användare. Om du inte befinner dig i någon av de här rollerna ber du administratören att lägga till dig i en av de här rollerna eller att skapa det nya användar kontot åt dig.
2. Kontrol lera att användar namnet finns i en domän som verifieras i din Azure AD. Om du inte har några verifierade domän namn i din Azure AD kan du använda din initiala Azure AD-domän, som slutar med *. onmicrosoft.com.
3. Kontrol lera att användar namnet finns i en domän som inte är federerad för Azure AD från din lokala annons. Det går inte att lägga till användare i molnet med domän namn som inte är inkluderade i lokal.
4. Kontrol lera att ingen annan användare eller kontakt har redan det användar namn som du vill tilldela den nya användaren. Användar namn måste vara unika i Azure AD.
5. Se [Azure AD-roller och-administratörer](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) för din Azure AD.
6. Se [domän namnen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) för din Azure AD.
7. Granska [gransknings loggar](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) för att visa mer detaljerad information om en nyligen skapad eller borttagen användare som utförde åtgärden och när.
8. Mer information om hur du lägger till nya användare finns i [använda Azure-portalen för att skapa en ny användare i din Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Mer information om administratörs behörigheter i Azure AD finns i [Administratörs roller för Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Information om hur du skapar en användare med Azure AD PowerShell finns i [Azure AD PowerShell för att skapa en ny användare](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem med självbetjänings registrering**

Utför följande steg för att felsöka problem med självbetjänings registrering:

1. För att använda självbetjäning med dina program måste du först aktivera själv registrering för din klient organisation. 
2. För att aktivera att ett program har stöd för självbetjänings registrering kan du lägga till det i ditt användar flöde. Nästa gång du går till inloggnings sidan för det programmet visas ett alternativ **_inget konto? Skapa ett!_* _. Då startas själv registrerings processen.
3. Information om hur du använder själv service registreringen för att fylla i en organisation i Azure AD finns i [själv registrering för Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. När du kopplar användar flödet till ett eller flera program kan användare som besöker programmet registrera sig och skaffa ett gäst konto med hjälp av de alternativ som har kon figurer ATS i användar flödet. För mer information om att registrera dig och skaffa ett gäst konto kan användarna se [själv registrering för gäst användare](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problem med att bjuda in en extern användare**

Så här felsöker du problem med att bjuda in en extern användare:

Se till att du skickar en användares inbjudan till e-postadressen som matchar namnet som användaren loggar in med. Om du skickar inbjudan till en användares e-postadress kan användaren inte lösa in den. Mer information finns i [dokumentationen till Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Jag kan inte tilldela licenser till en användare**

Så här felsöker du problem med att tilldela licenser till en användare:

1. För att hantera användar licenser bör du kontrol lera att du använder ett konto hos någon av de administratörs roller som krävs: global administratör, licens administratör eller användar administratör. Du kan kontrol lera användarens roll på fliken **katalog roll** i användarens blad.
2. Om du inte kan använda Azure-portalen och licens tilldelningen klickar du på meddelandet i det övre högra hörnet. Då öppnas bladet med information om vad som gick fel. I de flesta fall är det tillräckligt nog att förstå och lösa problemet.
3. Innan du kan tilldela en licens till en användare kontrollerar du att egenskapen **användnings plats** är inställd för användaren. Kontrol lera att användaren har egenskapen inställd genom att titta på fliken **profil** i användar bladet.
4. Se till att det finns tillräckligt med licenser för produkten som du vill tilldela. Du kan se antalet tillgängliga licenser i Azure-portalen på Azure [Active Directory-> licenser – > alla produkter](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Användaren kanske redan har en licens vars tjänster står i konflikt med de i den nya licens som du försöker tilldela. Om användaren till exempel har tjänsten Exchange Online (abonnemang 1) aktive rad kan du inte tilldela en licens till Exchange Online (abonnemang 2). Inaktivera en av tjänsterna för att tillåta den nya licens tilldelningen. Om du använder Azure-portalen eller PowerShell-cmdlets visas en lista med de tjänster som orsakar konflikten på sidan **problem information** .
6. Om du försöker ta bort en licens och det inte fungerar kan användaren ha andra licenser med tjänster som är beroende av de tjänster du försöker ta bort. Om du använder Azure-eller PowerShell-cmdlets visas en lista med de specifika tjänster som har beroenden.
7. Om du vill förstå varför en licens lades till eller togs bort från en användare (till exempel om du har gjort ändringar i organisationen) kontrollerar du gransknings loggarna. Ställ in filtret på **licens aktiviteter** för att visa alla ändringar, inklusive "aktören" som utförde dem.
8. Om du använder Exchange Online kan vissa användare i klient organisationen vara felaktigt konfigurerade med samma proxyserveradress. I sådana fall kan allmänna fel meddelanden visas när en licens åtgärd Miss lyckas. I [den här artikeln](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) finns mer information om det här problemet, inklusive information om [hur du ansluter till Exchange Online med fjärr-PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). För att identifiera vilka användare i klient organisationen som har samma proxyadress, kör du denna Exchange Online-cmdlet:

Använda

Get-Recipient | där {$ _. Postadresser '-match <user principal name> } | fL-namn, RecipientType, postadresser '





