---
title: Kryptera vissa e-postmeddelanden automatiskt från Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749455"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="c3a5b-102">Kryptera vissa e-postmeddelanden automatiskt från Office 365</span><span class="sxs-lookup"><span data-stu-id="c3a5b-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="c3a5b-103">Välj [E-postflödesregler](https://outlook.office365.com/ecp/)i **administrationscentret för** Exchange > .</span><span class="sxs-lookup"><span data-stu-id="c3a5b-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c3a5b-104">Klicka på **ikonen Nytt (+)** och klicka sedan på Tillämpa meddelandekryptering och **rättighetsskydd i Office 365 för meddelanden.**</span><span class="sxs-lookup"><span data-stu-id="c3a5b-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c3a5b-105">Ange **ett** namn för regeln i Namn, till exempel *Kryptera alla meddelanden*.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="c3a5b-106">I **Använd den här regeln om** väljer du **[Använd för alla meddelanden]**.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="c3a5b-107">Klicka på **Markera ett bredvid** Gör följande **fält.**</span><span class="sxs-lookup"><span data-stu-id="c3a5b-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="c3a5b-108">I den **nedrullningsmenyn** för RMS-mallen väljer **du Kryptera** och klickar sedan på **OK.**</span><span class="sxs-lookup"><span data-stu-id="c3a5b-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c3a5b-109">(Om du inte ser det här alternativet innebär det att din plan inte innehåller automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c3a5b-110">Men du kan lägga till den!)</span><span class="sxs-lookup"><span data-stu-id="c3a5b-110">But you can add it!)</span></span>
7. <span data-ttu-id="c3a5b-111">Markera **kryssrutan Granska den här regeln med allvarlighetsnivå** och välj sedan önskad nivå.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="c3a5b-112">Om ditt företag har avtalsmässiga skyldigheter att skicka krypterade e-postmeddelanden rekommenderar jag att ställa in nivån **på Hög.**</span><span class="sxs-lookup"><span data-stu-id="c3a5b-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="c3a5b-113">Klicka **på Framtvinga under Välj** en modell för **regeln.**</span><span class="sxs-lookup"><span data-stu-id="c3a5b-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="c3a5b-114">Välj valfritt val (i en lista med valfria val som du kan göra i det här läget. Många av dem kan lämnas med standardinställningen för enkelhetens skull).</span><span class="sxs-lookup"><span data-stu-id="c3a5b-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c3a5b-115">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c3a5b-116">Du kan alltid gå tillbaka och redigera regeln senare.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c3a5b-117">Mer information om hur du skapar regler för kryptering finns i [Definiera e-postflödesregler för att kryptera e-postmeddelanden i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="c3a5b-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

