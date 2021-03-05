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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484045"
---
# <a name="configuring-the-provision-service"></a>Konfigurera etableringstjänsten

För att automatisera användaretablering ska fungera kräver Azure AD giltiga autentiseringsuppgifter som gör att det går att ansluta till API för arbetsdagar-webbtjänster. Dessutom verifierar knappen Testanslutning i workday till AD-appen för användaretablering även om den kan ansluta till Azure AD Connect Provisioning Agent som är kopplad till AD-domänen.

Om Azure Portal returnerar ett fel när du sparar autentiseringsuppgifterna följer du de rekommenderade stegen nedan:

1. Bekräfta att du har konfigurerat användarkontot för Workday Integration System enligt i avsnittet Konfigurera [integreringssystemanvändare under Arbetsdagar.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Kontrollera att Azure AD Connect Provisioning Agent Service är igång på din lokala Windows-server med services managementkonsolen. Du kan också kontrollera status för agenten i Azure-portalen genom att klicka på knappen Visa lokala agenter.
3. Se till att du anger värdet för fältet "Användarnamn på arbetsdag" i formatet username@workday-klientorganisationsnamn. Om arbetsdagens klientorganisationsnamn saknas misslyckas autentiseringen arbetsdagar.
4. Om du konfigurerar integreringen med workday-implementeringsklientorganisationen noterar du de schemalagda avbrottstimmarna för din arbetsdag-klientorganisation. Arbetsdagar har planerat nedtid för sina implementeringsklienter under helger (vanligtvis från fredags kväll till lördag morgon) och anslutningsproblem under det här avbrottsfönstret är ett känt problem som automatiskt löses så snart implementeringsklienterna är online igen.
5. I sällsynta fall kan du även se det här felet om lösenordet för användaren av integrationssystemet har ändrats på grund av uppdatering av klientorganisationen eller om kontot är i låst eller utgånget läge. Kontrollera statusen för användaren av integrationssystemet med din arbetsdagarsadministratör.

Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
