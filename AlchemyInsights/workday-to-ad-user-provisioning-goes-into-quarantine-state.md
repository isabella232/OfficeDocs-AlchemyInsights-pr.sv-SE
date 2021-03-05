---
title: Arbetsdagar till AD-användaretablering sätts i karantän
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482905"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Arbetsdagar till AD-användaretablering sätts i karantän

**Arbetsdagar till AD-användaretablering sätts i karantän och inga användare skapas i AD**

Jobbet för etablering av användare i AD har satts i karantän och granskningsloggarna visar exportfelhändelser med felmeddelandet **Fel: OperationsError-SvcErr: Ett åtgärdsfel inträffade. Ingen överordnad referens har konfigurerats för katalogtjänsten. Katalogtjänsten kan därför inte utfärda referenser till objekt utanför** den här skogen. Det här felet visas vanligtvis om OU för Active Directory-behållaren inte är korrekt inställd eller om det uppstår problem med uttrycksmappningen som används för **parentEstinguishedName.**

Kontrollera om det finns stavfel **i standard-OU:n** för parametern Nya användare. Kontrollera att den angivna OU:n redan finns i AD. Om du använder **parentDistinguishedName** i attributmappningen ska du se till att det alltid utvärderas till en känd behållare i AD-domänen. Kontrollera exporthändelsen i granskningsloggarna för att se det genererade värdet.

Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

