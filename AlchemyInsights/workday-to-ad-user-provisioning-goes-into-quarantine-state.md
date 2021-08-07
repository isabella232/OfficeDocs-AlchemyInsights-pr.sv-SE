---
title: Arbetsdagar till AD-användaretablering förs i karantän
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036510"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Arbetsdagar till AD-användaretablering förs i karantän

**Arbetsdagar till AD användaretablering hamnar i karantän och inga användare skapas i AD**

Arbetsdagar till AD-jobbet för användaretablering har satts i karantän och granskningsloggarna visar exportfelhändelser med felmeddelandet **Fel: OperationsError-SvcErr: Ett åtgärdsfel inträffade. Ingen överordnad referens har konfigurerats för katalogtjänsten. Katalogtjänsten kan därför inte utfärda referenser till objekt utanför den här skogen.** Det här felet visas vanligtvis om OU för Active Directory-behållaren inte är korrekt inställd eller om det uppstår problem med uttrycksmappningen som används för **parentEstinguishedName.**

Kontrollera parametern Standard-OU **för nya** användare om det finns skrivfel. Kontrollera att den angivna OU:n redan finns i AD. Om du använder **parentDistinguishedName** i attributmappningen, se till att det alltid utvärderas till en känd behållare i AD-domänen. Kontrollera händelsen Export i granskningsloggarna för att se det genererade värdet.

Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

