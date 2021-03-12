---
title: Problem med en resurs eller en tjänsts huvudnamn
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714461"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problem med en resurs eller en tjänsts huvudnamn

1. Om du precis har börjat beskriver program- och tjänsthuvudobjekten i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) programregistrering, programobjekt och tjänsthuvudnamn i Azure Active Directory: vad de är, hur de används och hur de är relaterade till varandra. Ett exempelscenario med flera innehavare visas också för att illustrera relationen mellan ett programs programobjekt och motsvarande tjänsts huvudobjekt.
2. Du kan läsa mer om relationen mellan program och tjänsthuvudnamn genom att läsa [program och tjänstens huvudobjekt i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Så här gör [du:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Använd portalen för att skapa ett Azure AD-program och ett huvudnamn för tjänsten som kan komma åt resurser och visa hur du skapar ett nytt Azure Active Directory- (Azure Active Directory) program och tjänsthuvudnamn som kan användas med den rollbaserade åtkomstkontrollen.
4. Med [tjänstens huvud-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kan du programmässigt hantera instanser av program och styra vad ett program kan göra i klientorganisationen.
5. [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.
6. [Skillnader i resurstyper mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) visar skillnaderna mellan Azure AD Graph- och Microsoft Graph-resurser. Den visar resurser som har olika namn eller inte är tillgängliga. dessutom resurser som är tillgängliga i betaversionen av Microsoft Graph men inte i v1.0-versionen.

**Problem med gästanvändare**

- [Snabbstart:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Lägg till gästanvändare i katalogen i Azure Portal visar hur du lägger till en ny gästanvändare i Azure AD-katalogen via Azure Portal, skickar en inbjudan och ser hur gästanvändarens inlösningsprocess ser ut.
- [Självstudiekurs: Skapa användarflöden i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) visar hur du skapar vissa rekommenderade användarflöden med hjälp av Azure-portalen. Om du letar efter information om hur du konfigurerar ett flöde för resursägares lösenordslösenord (ROPC) i programmet finns mer information i Konfigurera autentiseringsuppgifter för resursägare i Azure AD B2C.
