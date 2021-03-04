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
# <a name="gpo-deployment"></a><span data-ttu-id="6dbbf-102">GPO-distribution</span><span class="sxs-lookup"><span data-stu-id="6dbbf-102">GPO Deployment</span></span>

<span data-ttu-id="6dbbf-103">Inställningar för användar- och datorobjekt i Azure Active Directory DS (Azure AD DS) hanteras ofta med hjälp grupprincip objekt (GPOs).</span><span class="sxs-lookup"><span data-stu-id="6dbbf-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="6dbbf-104">Azure AD DS inkluderar inbyggda GPOs för AADDC-användarna och AADDC-datorernas behållare.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="6dbbf-105">Du kan anpassa dessa inbyggda GPOs för att konfigurera grupprinciper efter behov för din miljö.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="6dbbf-106">Medlemmar i azure AD DC-administratörsgruppen har administratörsbehörigheter för grupprinciper i Azure AD DS-domänen och kan även skapa anpassade GPOs och organisationsenheter.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="6dbbf-107">Mer information om grupprinciper och hur den fungerar finns i grupprincip [Översikt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="6dbbf-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="6dbbf-108">I en hybridmiljö synkroniseras inte grupprinciper som konfigurerats i en AD DS lokal miljö till Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="6dbbf-109">Om du vill definiera konfigurationsinställningar för användare eller datorer i Azure AD DS redigerar du en av standard-GPOs eller skapar ett anpassat GPO.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="6dbbf-110">I den [här grupprincip](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) kan du se hur du installerar grupprincip Management-verktygen, hur ton redigerar inbyggda GPOs och hur du skapar anpassade GPOs.</span><span class="sxs-lookup"><span data-stu-id="6dbbf-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
