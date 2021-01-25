---
title: SCIM konfigurations problem
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949949"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="f6efa-102">SCIM konfigurations problem</span><span class="sxs-lookup"><span data-stu-id="f6efa-102">SCIM provisioning issue</span></span>

<span data-ttu-id="f6efa-103">Automatisk etablering syftar till att skapa användar identiteter och roller i de moln program som användare behöver åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="f6efa-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="f6efa-104">Förutom att skapa användar identiteter inkluderar automatisk etablering de underhåll och borttagningar av användar identitet som status eller roller förändras.</span><span class="sxs-lookup"><span data-stu-id="f6efa-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="f6efa-105">Innan du börjar med en distribution kan du se [hur etableringen fungerar](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) för att lära dig hur Azure Active Directory (AD) tillhandahåller och få konfigurations rekommendationer.</span><span class="sxs-lookup"><span data-stu-id="f6efa-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="f6efa-106">Som programutvecklare kan du använda systemet för SCIM (Cross-Domain Identity Management) för att aktivera automatisk etablering av användare och grupper mellan programmet och Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6efa-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="f6efa-107">Med [skapa en scim-slutpunkt och konfigurera användar etableringen med Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) -artikeln beskrivs hur du skapar en scim-slutpunkt och integrerar den med Azure AD etablerings tjänsten.</span><span class="sxs-lookup"><span data-stu-id="f6efa-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



