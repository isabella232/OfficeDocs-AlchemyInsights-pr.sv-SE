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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384843"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="8b3ec-102">Så här inaktiverar du externa grupper</span><span class="sxs-lookup"><span data-stu-id="8b3ec-102">How to disable External Groups</span></span>

<span data-ttu-id="8b3ec-103">Yammer externa meddelanden gäller Exchange transportregler (ETRs) av förebyggande kontroller för att förhindra företagsinformation från att delas.</span><span class="sxs-lookup"><span data-stu-id="8b3ec-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="8b3ec-104">För att hindra användare från att skapa externa grupper, måste du konfigurera en regel för Exchange transport (ETR) och konfigurera Yammer för att använda Exchange Transport-regel för att blockera externa meddelanden.</span><span class="sxs-lookup"><span data-stu-id="8b3ec-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="8b3ec-105">När du har skapat en regel i Exchange Online administratörscenter, gör så här om du vill ange ETR gäller i Yammer:</span><span class="sxs-lookup"><span data-stu-id="8b3ec-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="8b3ec-106">Logga in på Yammer som verifierad admin och i **Yammer administratörscenter**, gå till C **innehåll och säkerhet \> säkerhetsinställningar.**</span><span class="sxs-lookup"><span data-stu-id="8b3ec-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="8b3ec-107">Markera under **Externa meddelanden** **Tvinga din Exchange Online Exchange transportregler (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="8b3ec-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="8b3ec-108">Välj **Save**.</span><span class="sxs-lookup"><span data-stu-id="8b3ec-108">Choose **Save**.</span></span>

<span data-ttu-id="8b3ec-109">Mer information finns i [Kontrollera externa meddelanden i Yammer-nätverket med Exchange transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="8b3ec-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  