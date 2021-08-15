---
title: Problem med en enskild användare
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
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960169"
---
# <a name="problem-with-single-user"></a>Problem med en enskild användare

- Användaren kanske inte har etablerats eftersom tjänsten inte har haft möjlighet att utvärdera användaren ännu. Läs vägledningen för hur lång tid etablering tar samt förloppsfältet på konfigurationssidan för etablering. Om den stadiga statusen har angetts i avsnittet med ytterligare information innan datumet då användaren skapades/uppdaterades/togs bort, innebär det att vi inte har utvärderat användaren ännu. I det här scenariot är det bästa du kan göra att vänta tills etableringstjänsten slutförs.

  - Observera att vår tjänst endast är medveten om ändringar för en användare i källsystemet (Cloud HR). Det måste finnas en giltig ändring i källsystemet för att Azure AD ska kunna identifiera ändringen och föra den till Active Directory.
- Etableringstjänsten utvärderade användaren och bestämde att den inte bör etableras:
  - Om du har angett ett attributbaserat filter för scoping bör du kontrollera att användaren uppfyller de villkor som du har angett.
  - Om användarna redan finns i målsystemet och användarens status i käll- och målmatchning, kommer vi inte att vidta någon ytterligare åtgärd.
- Etableringstjänsten försökte etablera användaren och misslyckades. För de här scenarierna granskar du fliken felsökning och rekommendationer i etableringsloggarna:
  - Ett obligatoriskt attribut för användaren kanske saknas i lokal Active Directory eller Azure AD. Till exempel genererar inte reglerna för userPrincipalName eller sAMAccountName rätt värde.
  - Det matchande attributet (vanligtvis anställningsid) löser inte mot en unik användare i lokal Active Directory eller Azure AD. Det finns till exempel två användare med samma anställningsnr i AD och tjänsten returnerar en felkod som anger dubblettmålposter för samma källpost.

Om du vill granska loggar för enskild användare och grupper går [du till Granska etableringsloggarna för ett problem med en viss användare.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
