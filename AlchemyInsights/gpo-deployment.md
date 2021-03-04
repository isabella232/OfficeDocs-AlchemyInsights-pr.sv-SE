---
title: GPO-distribution
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428051"
---
# <a name="gpo-deployment"></a>GPO-distribution

Inställningar för användar- och datorobjekt i Azure Active Directory DS (Azure AD DS) hanteras ofta med hjälp grupprincip objekt (GPOs). Azure AD DS inkluderar inbyggda GPOs för AADDC-användarna och AADDC-datorernas behållare. Du kan anpassa dessa inbyggda GPOs för att konfigurera grupprinciper efter behov för din miljö. Medlemmar i azure AD DC-administratörsgruppen har administratörsbehörigheter för grupprinciper i Azure AD DS-domänen och kan även skapa anpassade GPOs och organisationsenheter. Mer information om grupprinciper och hur den fungerar finns i grupprincip [Översikt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I en hybridmiljö synkroniseras inte grupprinciper som konfigurerats i en AD DS lokal miljö till Azure AD DS. Om du vill definiera konfigurationsinställningar för användare eller datorer i Azure AD DS redigerar du en av standard-GPOs eller skapar ett anpassat GPO.

I den [här grupprincip](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) kan du se hur du installerar grupprincip Management-verktygen, hur ton redigerar inbyggda GPOs och hur du skapar anpassade GPOs.
