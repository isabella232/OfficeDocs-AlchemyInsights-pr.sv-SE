---
title: Användarhanteringsproblem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037510"
---
# <a name="user-management-issues"></a>Användarhanteringsproblem

**Vad händer med aktuella tilldelade användare i programmet om jag inaktiverar egenskapen "Användartilldelning krävs" (ange den här egenskapen till Nej)?**

Inaktivering **av obligatorisk användartilldelning** påverkar INTE de användare som för närvarande är tilldelade. Om du inaktiverar den här egenskapen kan bara alla användare få åtkomst till programmet. Alla listade användare och de användare som tilldelats grupper i programmet kommer fortfarande att vara giltiga.

- Information om hur du begränsar appen till vissa användare finns i Begränsa Azure AD-appen till en uppsättning användare – Plattform för [Microsoft-identitet | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- Om du vill tilldela användare och grupper till företagsprogram i Azure Active Directory (Azure AD), antingen från Azure-portalen eller med hjälp av PowerShell, kan du gå till Hantera användartilldelning för en app i [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Information om att delegera behörigheter för att skapa och hantera program finns i [Behörigheter för administratör för hantering av ombud för program – Azure AD | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **Dölj specifika företagsprogram för användare** – Använd följande steg för att dölja alla Microsoft 365-program från **panelen Mina** appar. Programmen kommer fortfarande att visas på Office 365-portalen.

 1. Logga in på Azure Portal som global administratör för katalogen. 
 2. Välj **Azure Active Directory.** 
 3. Välj **Användare**. 
 4. Välj **Användarinställningar.** 
 5. Klicka **på Hantera** hur **slutanvändarna startar och visar sina program under Företagsprogram.** 
 6. För **Användare kan bara se Office 365-program i Office 365-portalen klickar** du på **Ja.** 
 7. Klicka på **Spara**. 
 8. Mer information finns i [Dölja ett företagsprogram för användare i Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Om du erbjuder en SaaS-app (programvara som en tjänst) till många organisationer kan du konfigurera appen så att inloggningar accepteras från valfri Azure Active Directory-klientorganisation (Azure AD). Den här konfigurationen kallas för att "göra programmet till flera innehavare". Användare i alla Azure AD-klientorganisationen kommer att kunna logga in på appen när de har gett sitt medgivande för att använda sitt konto med din app. Mer information finns i Skapa [appar som loggar in Azure AD-användare – Microsoft identity platform | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **Hur kan en slutanvändare komma åt programmet när han eller hon har tilldelats till programmet?**

Varje app i enterprise-programbladet har en länk som slutanvändarna kan komma åt. Användare kan också komma åt appen via **Myapps-portalen** på ett enkelt sätt.

- **Vill du veta vilka program och typer av program som används av användarna?**

Du kan hämta inloggningsrapporter för de senaste 30 dagarna från att portal.azure.com > Azure Active Directory> **Inloggningar> ladda ned rapporter**.

- Läs om hur [du beviljar administratörsmedgivande för hela klientorganisationen till ett program](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) och Konfigurera hur [slutanvändarna ger sitt medgivande till programmen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Förstå [hur medgivande fungerar och](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Hantera medgivande till [program.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


