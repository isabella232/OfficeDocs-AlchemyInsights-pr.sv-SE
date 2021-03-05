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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482914"
---
# <a name="user-provisioning"></a>Användaretablering

- Använd [etableringsfunktioner på begäran för](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) att etablera en användare och få detaljerad diagnostik om stegen som vidtas.
- Information om hur du felsöker problem som uppstår när användare och grupper etableras finns i [felsökningsguiden Inga användare etableras.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Om du observerar att användare inte etableras, se [Etableringsloggar (förhandsversion)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) i Azure Active Directory (AD). Sök efter loggposter som gäller för en viss användare.
- Starta om etableringen regelbundet för att se alla användare som har missats i en tidigare etableringscykel.
- Användaren/gruppen kanske inte har etablerats eftersom vår tjänst inte har haft möjlighet att utvärdera användaren ännu. Läs vägledningen för hur lång tid etableringen tar samt förloppsfältet på konfigurationssidan för etablering. Om den stadiga statusen som anges i avsnittet med ytterligare information ligger före datumet då användaren skapades/uppdaterades/togs bort, innebär det att vi inte har utvärderat användaren ännu. I det här scenariot är det bäst att vänta till etableringstjänsten slutförs. Om du har uppnått det stadiga läget rekommenderar vi att du gör en omstart från användargränssnittet i Azure Portal.
  - Observera att vår tjänst endast är medveten om ändringar för en användare/grupp i källsystemet (Azure Active Directory). Om en användare/grupp tas bort direkt i programmet (till exempel ServiceNow) känner vi inte till ändringarna och kan inte återställa dem beroende på användarens status i källsystemet. I det här scenariot är det bäst att återställa ändringen direkt i målprogrammet.
- Vår tjänst utvärderade användaren/gruppen och kom fram till att den inte bör tillhandahållas:
  - Om du har angett omfattningen till tilldelade användare och grupper kontrollerar du om användaren/gruppen har tilldelats till programmet.
  - Om användaren/gruppen har tilldelats till programmet ska du kontrollera att de inte har tilldelats standardåtkomstrollen. Den här rollen kan inte användas för etablering.
  - Om du har angett ett attributbaserat filter, kontrollera att användaren uppfyller de villkor som du har angett.
  - Om användarna redan finns i målsystemet och användarens status i källan och målmatchning kommer vi inte att vidta någon ytterligare åtgärd.
- Tjänsten försökte etablera användaren och misslyckades. För dessa scenarier granskar du fliken felsökning och rekommendationer i etableringsloggarna:
  - Ett obligatoriskt attribut för användaren kanske saknas i Azure Active Directory eller inte matchar formatet som krävs av tredjepartsprogrammet. Till exempel kan attributet Land för en användare ställas in på USA när det ska vara USA.
  - Attributet är ett referensattribut som ännu inte finns i målprogrammet. Ett referensattribut är ett attribut som pekar på ett annat objekt, till exempel en användare som är medlem i en grupp. Användarens ID skulle finnas i medlemsattributet för gruppen, men kan bara bearbetas om användarobjektet som det pekar på redan finns.
