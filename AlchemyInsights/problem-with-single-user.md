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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430208"
---
# <a name="problem-with-single-user"></a>Problem med en enskild användare

- Användaren kanske inte har etablerats eftersom tjänsten inte har haft möjlighet att utvärdera användaren ännu. Läs vägledningen för hur lång tid etableringen tar samt förloppsfältet på konfigurationssidan för etablering. Om den stadiga statusen som anges i avsnittet med ytterligare information ligger före datumet då användaren skapades/uppdaterades/togs bort, innebär det att vi inte har utvärderat användaren ännu. I det här scenariot är det bäst att vänta till etableringstjänsten slutförs.

  - Observera att vår tjänst endast är medveten om ändringar för en användare i källsystemet (Cloud HR). Det måste göras en giltig ändring i källsystemet för att Azure AD ska kunna identifiera ändringen och föra den till Active Directory.
- Etableringstjänsten utvärderade användaren och kom fram till att den inte bör tillhandahållas:
  - Om du har angett ett attributbaserat filter, kontrollera att användaren uppfyller de villkor som du har angett.
  - Om användarna redan finns i målsystemet och användarens status i källan och målmatchning kommer vi inte att vidta någon ytterligare åtgärd.
- Etableringstjänsten försökte etablera användaren och misslyckades. För dessa scenarier granskar du fliken felsökning och rekommendationer i etableringsloggarna:
  - Ett obligatoriskt attribut för användaren kanske saknas i lokal Active Directory eller Azure AD. Till exempel skapar inte reglerna för userPrincipalName eller sAMAccountName rätt värde.
  - Det matchande attributet (vanligtvis employeeId) löser inte mot en unik användare i en lokal Active Directory eller Azure AD. Det finns till exempel två användare med samma anställningsnr i AD och tjänsten returnerar en felkod som anger dubblettmålposter för samma källpost.

Om du vill granska loggar för enskild användare och grupper kan du [läsa i etableringsloggarna för ett problem med en viss användare.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
