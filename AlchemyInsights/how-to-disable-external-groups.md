---
title: Så här inaktiverar du externa grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704146"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d2d7a-102">Så här inaktiverar du externa grupper</span><span class="sxs-lookup"><span data-stu-id="d2d7a-102">How to disable External Groups</span></span>

<span data-ttu-id="d2d7a-103">I externa meddelanden i Yammer används Exchange Transport Rules (ETR), en uppsättning proaktiva kontroller för att förhindra att företags informationen delas.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="d2d7a-104">För att hindra användare från att skapa externa grupper måste du konfigurera en Exchange-Exchange och sedan konfigurera Yammer så att externa meddelanden blockeras.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="d2d7a-105">När du har skapat en regel i administrations centret för Exchange Online följer du de här stegen för att ange att Exchange ska tillämpas i Yammer:</span><span class="sxs-lookup"><span data-stu-id="d2d7a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d2d7a-106">Logga in på Yammer som verifierad administratör och gå till **säkerhet och säkerhets \> Inställningar** i **administrations centret för Yammer**.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="d2d7a-107">Under **externa meddelanden**väljer **du tvinga fram Exchange-ETR för Exchange Online i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="d2d7a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="d2d7a-108">Välj **Save**.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-108">Choose **Save**.</span></span>

<span data-ttu-id="d2d7a-109">Mer information finns i [inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="d2d7a-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  