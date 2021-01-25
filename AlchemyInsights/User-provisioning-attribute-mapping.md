---
title: Mappning av attributmappning
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949897"
---
# <a name="user-provisioning-attribute-mapping"></a>Mappning av attributmappning

1. Information om hur du felsöker problem med kända attribut finns i [attribut mappningar](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) tillhandahåller stöd för användar konfiguration för SaaS program från tredje part, till exempel Salesforce, G Suite och andra. Om du aktiverar användar konfiguration för ett SaaS program från tredje part styr Azure-portalen dess attributvärden via Attribute-mappningar. Information om hur du anpassar standardattributen för mappning finns i [Anpassa attribut för användar hantering för SaaS-program i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Om du vill veta mer om hur du konfigurerar SaaS app User kan du läsa [Vad är automatiserad SaaS app User-etablering i Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. När du anpassar attribut-mappningar för användar etableringen kanske du upptäcker att det attribut som du vill mappa inte finns med i listan source Attribute. [Synkroniseringen av ett attribut från din lokala Active Directory till Azure AD för etablering till en program](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikel visar hur du lägger till ett saknat attribut genom att synkronisera det från din lokala annons till Azure AD.
