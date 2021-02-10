---
title: Synkronisering av lösenordshashar för domäntjänst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177620"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="34bbd-102">Synkronisering av lösenordshashar för domäntjänst</span><span class="sxs-lookup"><span data-stu-id="34bbd-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="34bbd-103">**Om din Azure AD DS-instans uppmanar dig att aktivera synkronisering av lösenordshashar**</span><span class="sxs-lookup"><span data-stu-id="34bbd-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="34bbd-104">Du stöter på ett scenario där du kör en hybridmiljö med användare som synkroniserar från en lokal Azure Active Directory DS-miljö (AD DS).</span><span class="sxs-lookup"><span data-stu-id="34bbd-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="34bbd-105">Det här scenariot påträffas trots att du har synkronisering av lösenordshashar från den lokala AD DS till Azure AD-klienten.</span><span class="sxs-lookup"><span data-stu-id="34bbd-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="34bbd-106">**Orsak**</span><span class="sxs-lookup"><span data-stu-id="34bbd-106">**Cause**</span></span>

<span data-ttu-id="34bbd-107">Det här händer eftersom Azure AD Connect som standard inte synkroniserar äldre NTLM-lösenordshanterare (New Technology LAN Manager) och Kerberos-lösenordshashar som krävs för Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="34bbd-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="34bbd-108">**Lösning**</span><span class="sxs-lookup"><span data-stu-id="34bbd-108">**Workaround**</span></span> 

<span data-ttu-id="34bbd-109">Du måste konfigurera Azure AD Connect för att synkronisera de lösenordshashar som krävs för NTLM- och Kerberos-autentisering.</span><span class="sxs-lookup"><span data-stu-id="34bbd-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="34bbd-110">När Azure AD Connect har konfigurerats synkroniseras sedan även äldre lösenordshashar till Azure AD vid skapande av lokalt konto eller ändring av lösenord.</span><span class="sxs-lookup"><span data-stu-id="34bbd-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="34bbd-111">Mer information [om](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) detta och anvisningar om hur du aktiverar lösenordssynkronisering i Azure AD DS hybridmiljöer finns här.</span><span class="sxs-lookup"><span data-stu-id="34bbd-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>