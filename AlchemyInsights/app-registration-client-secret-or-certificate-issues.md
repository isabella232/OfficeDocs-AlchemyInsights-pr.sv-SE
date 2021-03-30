---
title: Problem med appregistreringsklienthemlighet eller certifikat
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405331"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problem med appregistreringsklienthemlighet eller certifikat

Går programhemligheten ut?

Oavsett hur det registrerade programmet skapades, oavsett om det är genom standardregistreringsprocessen i registreringsportalen för appar eller om Service Principal skapades i klientorganisationen med hjälp av programmedgivande, måste en ny klienthemlighet skapas före utgångsdatumet för den aktuella och uppdateras i den relaterade programkoden. Max giltighetsperioden är 2 år. Som en påminnelse måste det hemliga värdet registreras eftersom det inte längre visas när du lämnar registreringssidan för appen i portalen. Mer information finns i [Snabbstart: Registrera en app på Microsoft-identitetsplattformen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) och [Metodtips för Microsofts identitetsplattform.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Mer information finns i Skapa [en Azure AD-app & tjänstens huvudnamn i portalen – Microsoft-identitetsplattformen.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
