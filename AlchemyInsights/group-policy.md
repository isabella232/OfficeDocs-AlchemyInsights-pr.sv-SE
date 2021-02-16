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
# <a name="group-policy"></a><span data-ttu-id="ff76f-102">Grupprincip</span><span class="sxs-lookup"><span data-stu-id="ff76f-102">Group policy</span></span>

<span data-ttu-id="ff76f-103">Inställningar för användar- och datorobjekt i Azure Active Directory DS (Azure AD DS) hanteras ofta med grupprincip objekt (GPOs).</span><span class="sxs-lookup"><span data-stu-id="ff76f-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="ff76f-104">Azure AD DS inkluderar inbyggda GPOs för AADDC-användarna och AADDC-datorernas behållare.</span><span class="sxs-lookup"><span data-stu-id="ff76f-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="ff76f-105">Du kan anpassa dessa inbyggda GPOs för att konfigurera grupprinciper efter behov för din miljö.</span><span class="sxs-lookup"><span data-stu-id="ff76f-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="ff76f-106">Medlemmar i azure AD DC-administratörsgruppen har administratörsbehörigheter för grupprinciper i Azure AD DS-domänen och kan även skapa anpassade GPOs och organisationsenheter.</span><span class="sxs-lookup"><span data-stu-id="ff76f-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="ff76f-107">Mer information om grupprinciper och hur den fungerar finns i grupprincip [översikt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="ff76f-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="ff76f-108">I en hybridmiljö synkroniseras inte grupprinciper som konfigurerats i en AD DS lokal miljö till Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="ff76f-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="ff76f-109">Om du vill definiera konfigurationsinställningar för användare eller datorer i Azure AD DS redigerar du en av standard-GPOs eller skapar ett anpassat GPO.</span><span class="sxs-lookup"><span data-stu-id="ff76f-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="ff76f-110">Den här [grupprincip](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) visar hur du installerar grupprincip Management-verktygen, hur ton redigerar inbyggda GPOs och hur du skapar anpassade GPOs.</span><span class="sxs-lookup"><span data-stu-id="ff76f-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



