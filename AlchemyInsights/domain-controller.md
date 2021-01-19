---
title: Domänkontrollant
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901315"
---
# <a name="domain-controller"></a><span data-ttu-id="91fe9-102">Domänkontrollant</span><span class="sxs-lookup"><span data-stu-id="91fe9-102">Domain controller</span></span>

<span data-ttu-id="91fe9-103">**Det går inte att aktivera AAD-DS eller distributionen fungerar inte**</span><span class="sxs-lookup"><span data-stu-id="91fe9-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="91fe9-104">Utför följande steg för att lösa problemet med att Azure AD Domain Service (AAD-DS) inte aktive ras eller att det inte går att distribueras:</span><span class="sxs-lookup"><span data-stu-id="91fe9-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="91fe9-105">Om du använder ett befintligt virtuellt nätverk kontrollerar du dina NSG för regler som blockerar de portar som behövs för att synkroniseras i AAD-DS i portalen https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="91fe9-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="91fe9-106">Kontrol lera om fel meddelandet besvaras i den här fel söknings guiden som är tillgänglig i  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="91fe9-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="91fe9-107">Försök Distribuera Azure AD Domain Services i ett nytt virtuellt nätverk.</span><span class="sxs-lookup"><span data-stu-id="91fe9-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="91fe9-108">Följ start guiden för hur du distribuerar AAD-DS, som finns i [själv studie kurs för att skapa Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="91fe9-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="91fe9-109">Om du har problem med distributionen av Azure AD Domain Services läser du [Felsöka Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) för att lösa vanliga fel för att få saker att fungera igen.</span><span class="sxs-lookup"><span data-stu-id="91fe9-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="91fe9-110">**Det går inte att inaktivera AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="91fe9-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="91fe9-111">AAD – kunde inte pausas.</span><span class="sxs-lookup"><span data-stu-id="91fe9-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="91fe9-112">Om du vill sluta använda den hanterade domänen måste den tas bort.</span><span class="sxs-lookup"><span data-stu-id="91fe9-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="91fe9-113">Om du stöter på problem, löser vanliga fel meddelanden och tillhör ande fel söknings steg som hjälper dig att komma igång igen, se [Felsöka Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="91fe9-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
