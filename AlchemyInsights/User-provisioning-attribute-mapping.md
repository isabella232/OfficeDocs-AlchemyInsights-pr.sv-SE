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
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="dee95-102">Mappning av attributmappning</span><span class="sxs-lookup"><span data-stu-id="dee95-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="dee95-103">Information om hur du felsöker problem med kända attribut finns i [attribut mappningar](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="dee95-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="dee95-104">Microsoft Azure Active Directory (AD) tillhandahåller stöd för användar konfiguration för SaaS program från tredje part, till exempel Salesforce, G Suite och andra.</span><span class="sxs-lookup"><span data-stu-id="dee95-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="dee95-105">Om du aktiverar användar konfiguration för ett SaaS program från tredje part styr Azure-portalen dess attributvärden via Attribute-mappningar.</span><span class="sxs-lookup"><span data-stu-id="dee95-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="dee95-106">Information om hur du anpassar standardattributen för mappning finns i [Anpassa attribut för användar hantering för SaaS-program i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="dee95-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="dee95-107">Om du vill veta mer om hur du konfigurerar SaaS app User kan du läsa [Vad är automatiserad SaaS app User-etablering i Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="dee95-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="dee95-108">När du anpassar attribut-mappningar för användar etableringen kanske du upptäcker att det attribut som du vill mappa inte finns med i listan source Attribute.</span><span class="sxs-lookup"><span data-stu-id="dee95-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="dee95-109">[Synkroniseringen av ett attribut från din lokala Active Directory till Azure AD för etablering till en program](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikel visar hur du lägger till ett saknat attribut genom att synkronisera det från din lokala annons till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dee95-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
