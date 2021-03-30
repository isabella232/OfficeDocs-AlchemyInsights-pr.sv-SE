---
title: API-behörigheter och medgivandeprocess
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405442"
---
# <a name="api-permissions-and-consent-process"></a>API-behörigheter och medgivandeprocess

För att appen ska få åtkomst till data i Microsoft Graph måste användaren eller administratören ge det rätt behörigheter via en medgivandeprocess. [I Microsoft Graph-behörighetsreferensen](https://docs.microsoft.com/graph/permissions-reference) visas behörigheterna som är kopplade till varje huvuduppsättning Av Microsoft Graph-API:er. Den innehåller även vägledning om hur du använder behörigheterna.

**Konfigurera eller uppdatera tjänstens huvudnamn**

- [Skapa serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – i den här artikeln beskrivs hur du skapar ett nytt servicePrincipal-objekt.
- Skapa ett [Azure AD-program](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) &-tjänstens huvudnamn i portalen – Den här artikeln visar hur du skapar ett nytt Azure Active Directory-program och ett azure AD-program (Azure AD) som kan användas med den rollbaserade åtkomstkontrollen.
- [Appar & tjänsthuvudnamn](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) i Azure AD – I den här artikeln beskrivs programregistrering, programobjekt och tjänsthuvudnamn i Azure Active Directory: vad de är, hur de används och hur de är relaterade till varandra.

**Lägga till eller uppdatera appregistrering och ge administratörsmedgivande**

- [Skapa en appregistrering](https://docs.microsoft.com/graph/api/application-post-applications) – i den här artikeln visar vi hur du skapar ett nytt programobjekt.
- [Uppdatera en appregistrering – API-behörigheter](https://docs.microsoft.com/graph/api/application-update) – den här artikeln visar hur du uppdaterar egenskaperna för ett programobjekt.
- [Ge administratörsmedgivande](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – För administratörsmedgivande och medgivande i allmänhet kräver vi att en administratör uttryckligen beviljar medgivande.
- [RBAC (beta) –](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) Rollhanteringsbehållare för enhetliga rolldefinitioner och rolltilldelningar för Microsoft 365 RBAC-leverantörer som har stöd för flera huvudnamn och flera omfattningar i en enda rolltilldelning. Detta skiljer sig från *rbacApplication-resurstyp.* Microsoft Intune är ett exempel på en sådan RBAC-leverantör. En rolltilldelning i Intune kan ha en matris med huvudnamn och en matris med omfattningsgrupper. **Detta är i betaversion, vilket innebär att den fortfarande är under utveckling och inte rekommenderas för användning i produktion.**
