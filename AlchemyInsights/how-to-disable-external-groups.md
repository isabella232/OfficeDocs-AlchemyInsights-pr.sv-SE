---
title: Så här inaktiverar du externa grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739511"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="1176d-102">Så här inaktiverar du externa grupper</span><span class="sxs-lookup"><span data-stu-id="1176d-102">How to disable External Groups</span></span>

<span data-ttu-id="1176d-103">Yammer externa meddelanden gäller Exchange Transport regler (ETRs), en uppsättning proaktiva kontroller för att förhindra att företagsinformation delas.</span><span class="sxs-lookup"><span data-stu-id="1176d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="1176d-104">För att begränsa användare från att skapa externa grupper, måste du konfigurera en Exchange Transport-regel (ETR) och sedan konfigurera Yammer att använda Exchange Transport-regel för att blockera externa meddelanden.</span><span class="sxs-lookup"><span data-stu-id="1176d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="1176d-105">När du har skapat en regel i Exchange Online Admin Center, Följ dessa steg för att ange ETR ska tillämpas i Yammer:</span><span class="sxs-lookup"><span data-stu-id="1176d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="1176d-106">Logga in på Yammer som en verifierad administratör och i **Administrationscenter för Yammer**, gå till C **innehåll och \> säkerhet säkerhetsinställningar.**</span><span class="sxs-lookup"><span data-stu-id="1176d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="1176d-107">Under **externa meddelanden**, Välj **Framtvinga Exchange Online Exchange Transport-regler (ETRS) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="1176d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="1176d-108">Välj **Save**.</span><span class="sxs-lookup"><span data-stu-id="1176d-108">Choose **Save**.</span></span>

<span data-ttu-id="1176d-109">Mer information finns [i inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="1176d-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  