---
title: Användaretablering
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971357"
---
# <a name="user-provisioning"></a>Användaretablering

- Använd [etableringsfunktioner på begäran för att](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) tillhandahålla en användare och få detaljerad diagnostik om stegen som vidtas.
- Information om hur du felsöker problem som uppstår när användare och grupper etableras finns i [felsökningsguiden Inga användare etableras](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Om du observerar att användare inte etableras, se [Etableringsloggar (förhandsversion)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) i Azure Active Directory (AD). Sök efter loggposter som gäller en viss användare.
- Starta om etableringen regelbundet för att se alla användare som har missats i en tidigare etableringscykel.
- Användaren/gruppen kanske inte har etablerats eftersom tjänsten inte har haft möjlighet att utvärdera användaren ännu. Läs vägledningen för hur lång tid etablering tar samt förloppsfältet på konfigurationssidan för etablering. Om den stadiga statusen har angetts i avsnittet med ytterligare information innan datumet då användaren skapades/uppdaterades/togs bort, innebär det att vi inte har utvärderat användaren ännu. I det här scenariot är det bästa du kan göra att vänta tills etableringstjänsten slutförs. Om den stadiga statusen har uppnåtts rekommenderar vi att du gör en omstart från användargränssnittet i Azure-portalen.
  - Observera att tjänsten endast är medveten om ändringar för en användare/grupp i källsystemet (Azure Active Directory). Om en användare/grupp tas bort direkt i programmet (till exempel ServiceNow) känner vi inte till ändringarna och kan inte återställa den baserat på användarens status i källsystemet. I det här scenariot är det bäst att återställa ändringen direkt i målprogrammet.
- Tjänsten har utvärderat användaren/gruppen och fastställt att den inte ska tillhandahållas:
  - Om du har angett omfattningen till tilldelade användare och grupper kontrollerar du om användaren/gruppen har tilldelats till programmet.
  - Om användaren/gruppen har tilldelats till programmet bör du kontrollera att de inte har tilldelats standardåtkomstrollen. Den här rollen kan inte användas för etablering.
  - Om du har angett ett attributbaserat filter för scoping bör du kontrollera att användaren uppfyller de villkor som du har angett.
  - Om användarna redan finns i målsystemet och användarens status i käll- och målmatchning, kommer vi inte att vidta någon ytterligare åtgärd.
- Tjänsten försökte etablera användaren och misslyckades. För de här scenarierna granskar du fliken felsökning och rekommendationer i etableringsloggarna:
  - Ett obligatoriskt attribut för användaren kanske saknas i Azure Active Directory eller inte överensstämmer med det format som krävs av tredjepartsprogrammet. Till exempel kan attributet Land för en användare ställas in på USA när det ska vara USA.
  - Attributet är ett referensattribut som ännu inte finns i målprogrammet. Ett referensattribut är ett attribut som pekar på ett annat objekt, till exempel en användare som är medlem i en grupp. Användarens ID finns i medlemsattributet i gruppen, men kan bara bearbetas om användarobjektet det pekar på redan finns.
