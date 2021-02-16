---
title: Grupprincip
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256907"
---
# <a name="group-policy"></a>Grupprincip

Inställningar för användar- och datorobjekt i Azure Active Directory DS (Azure AD DS) hanteras ofta med grupprincip objekt (GPOs). Azure AD DS inkluderar inbyggda GPOs för AADDC-användarna och AADDC-datorernas behållare. Du kan anpassa dessa inbyggda GPOs för att konfigurera grupprinciper efter behov för din miljö. Medlemmar i azure AD DC-administratörsgruppen har administratörsbehörigheter för grupprinciper i Azure AD DS-domänen och kan även skapa anpassade GPOs och organisationsenheter. Mer information om grupprinciper och hur den fungerar finns i grupprincip [översikt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I en hybridmiljö synkroniseras inte grupprinciper som konfigurerats i en AD DS lokal miljö till Azure AD DS. Om du vill definiera konfigurationsinställningar för användare eller datorer i Azure AD DS redigerar du en av standard-GPOs eller skapar ett anpassat GPO.

Den här [grupprincip](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) visar hur du installerar grupprincip Management-verktygen, hur ton redigerar inbyggda GPOs och hur du skapar anpassade GPOs.



