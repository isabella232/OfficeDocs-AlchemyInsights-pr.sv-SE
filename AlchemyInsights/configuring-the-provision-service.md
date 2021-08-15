---
title: Konfigurera etableringstjänsten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033296"
---
# <a name="configuring-the-provision-service"></a>Konfigurera etableringstjänsten

För att automatisera användaretablering ska fungera kräver Azure AD giltiga autentiseringsuppgifter som gör att det kan ansluta till API för arbetsdagar webbtjänster. Dessutom verifierar knappen Testa anslutning i arbetsdagar till AD-appen för användaretablering även om den kan ansluta till Azure AD Anslut Provisioning Agent som är kopplad till AD-domänen.

Om Azure Portal returnerar ett fel när autentiseringsuppgifterna sparas följer du rekommenderade steg nedan:

1. Bekräfta att du har konfigurerat användarkontot för workday integration system enligt i självstudiekursen i [avsnittet Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Kontrollera att Azure AD Anslut Provisioning Agent Service är igång på den lokala e-Windows-servern med hjälp av Services Management Console. Du kan också kontrollera status för agenten i Azure Portal genom att klicka på knappen Visa lokala agenter.
3. Kontrollera att du anger värdet för fältet "Arbetsdagar, användarnamn" i det format username@workday-klientorganisationens namn. Om arbetsdagar-klientorganisationsnamn saknas misslyckas autentiseringen arbetsdagar.
4. Om du konfigurerar integreringen med en klientorganisation för arbetsdag-implementering bör du observera de schemalagda avbrottstiderna för din klientorganisations arbetsdag. Arbetsdagar har planerat ned tid för sina implementeringsklienter över helger (vanligtvis från fredag kväll till lördag morgon) och anslutningsproblem under detta avbrottsfönster är ett känt problem som automatiskt löses så snart implementeringsklienterna är online igen.
5. I sällsynta fall kan du även se det här felet om lösenordet till användaren av integrationssystemet har ändrats på grund av uppdatering av klientorganisationen eller om kontot är i låst eller utgånget läge. Kontrollera status för användaren av integrationssystemet med din arbetsdagar-administratör.

Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
