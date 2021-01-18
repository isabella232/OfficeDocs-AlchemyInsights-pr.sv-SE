---
title: Konfigurera LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885579"
---
# <a name="configure-ldap"></a><span data-ttu-id="abdac-102">Konfigurera LDAP</span><span class="sxs-lookup"><span data-stu-id="abdac-102">Configure LDAP</span></span>

<span data-ttu-id="abdac-103">Så här konfigurerar du LDAP:</span><span class="sxs-lookup"><span data-stu-id="abdac-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="abdac-104">Kontrol lera din domäns hälsa på [Azure-portalen](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="abdac-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="abdac-105">Se till att det finns en giltig Azure AD-prenumeration och Azure AD Domain Services har Aktiver ATS.</span><span class="sxs-lookup"><span data-stu-id="abdac-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="abdac-106">Det certifikat som krävs för att aktivera säker LDAP måste erhållas från en betrodd offentlig certifikat utfärdare eller vara ett självsignerat certifikat.</span><span class="sxs-lookup"><span data-stu-id="abdac-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="abdac-107">Kontrol lera att certifikatet följer de nödvändiga [rikt linjerna](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="abdac-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="abdac-108">**Ogiltigt certifikat**</span><span class="sxs-lookup"><span data-stu-id="abdac-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="abdac-109">Om du vill förnya ett certifikat följer du stegen för att skapa ett nytt certifikat och laddar upp det igen: [Konfigurera LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="abdac-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="abdac-110">Information om hur du löser kända problem med säkra LDAP-aviseringar i Azure Active Directory Domain Services finns i [lösa LDAP-varningar](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="abdac-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
