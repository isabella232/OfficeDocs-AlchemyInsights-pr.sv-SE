---
title: Inaktivera externa grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720786"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="c74e4-102">Inaktivera externa grupper</span><span class="sxs-lookup"><span data-stu-id="c74e4-102">How to disable External Groups</span></span>

<span data-ttu-id="c74e4-103">Yammer externa meddelanden tillämpar Exchange Transport Rules (ETRs), en uppsättning proaktiva kontroller för att förhindra att företagsinformation delas.</span><span class="sxs-lookup"><span data-stu-id="c74e4-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="c74e4-104">För att begränsa användare från att skapa externa grupper måste du konfigurera en Exchange-transportregel (ETR) och sedan konfigurera Yammer så att den använder Exchange Transport-regeln för att blockera externa meddelanden.</span><span class="sxs-lookup"><span data-stu-id="c74e4-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="c74e4-105">När du har skapat en regel i Administrationscentret för Exchange Online följer du dessa steg för att ange att ETR ska gälla i Yammer:</span><span class="sxs-lookup"><span data-stu-id="c74e4-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="c74e4-106">Logga in på Yammer som verifierad administratör och gå till **säkerhetsinställningarna \> för C-innehåll och säkerhet** i **Administrationscentret för Yammer.**</span><span class="sxs-lookup"><span data-stu-id="c74e4-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="c74e4-107">Under **Externa meddelanden**väljer du **Framtvinga dina ETR-regler för Exchange Online Exchange Transport (i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="c74e4-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="c74e4-108">Välj **Save**.</span><span class="sxs-lookup"><span data-stu-id="c74e4-108">Choose **Save**.</span></span>

<span data-ttu-id="c74e4-109">Mer information finns [i Inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="c74e4-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  