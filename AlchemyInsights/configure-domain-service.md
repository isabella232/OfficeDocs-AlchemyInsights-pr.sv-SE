---
title: Konfigurera domän tjänst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885686"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="800a9-102">Det går inte att aktivera AAD-DS eller distributionen fungerar inte</span><span class="sxs-lookup"><span data-stu-id="800a9-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="800a9-103">Utför följande steg för att lösa problemet med att Azure AD Domain Service (AAD-DS) inte aktive ras eller att det inte går att distribueras:</span><span class="sxs-lookup"><span data-stu-id="800a9-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="800a9-104">Om du använder ett befintligt virtuellt nätverk kontrollerar du dina NSG för regler som blockerar de portar som behövs för att synkroniseras i AAD-DS i portalen https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="800a9-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="800a9-105">Kontrol lera om fel meddelandet besvaras i den här fel söknings guiden som är tillgänglig i  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="800a9-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="800a9-106">Försök Distribuera Azure AD Domain Services i ett nytt virtuellt nätverk.</span><span class="sxs-lookup"><span data-stu-id="800a9-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="800a9-107">Följ start guiden för hur du distribuerar AAD-DS: [skapa och konfigurera AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="800a9-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="800a9-108">Om du har problem med distributionen av Azure AD Domain Services läser du [Felsöka Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) för att lösa vanliga fel för att få saker att fungera igen.</span><span class="sxs-lookup"><span data-stu-id="800a9-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="800a9-109">**Det går inte att inaktivera AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="800a9-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="800a9-110">AAD – kunde inte pausas.</span><span class="sxs-lookup"><span data-stu-id="800a9-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="800a9-111">Om du vill sluta använda den hanterade domänen måste den tas bort.</span><span class="sxs-lookup"><span data-stu-id="800a9-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="800a9-112">Information om hur du tar bort en hanterad domän finns i [ta bort AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="800a9-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



