---
title: Kryptera vissa e-postmeddelanden i Office 365 automatiskt
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749446"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="a9e6a-102">Kryptera vissa e-postmeddelanden i Office 365 automatiskt</span><span class="sxs-lookup"><span data-stu-id="a9e6a-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="a9e6a-103">Du kan automatiskt kryptera meddelanden som användare skickar till vissa externa personer eller organisationer.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="a9e6a-104">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="a9e6a-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="a9e6a-105">Välj [E-postflödesregler](https://outlook.office365.com/ecp/)i **administrationscentret för** Exchange > .</span><span class="sxs-lookup"><span data-stu-id="a9e6a-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a9e6a-106">Klicka på **ikonen Nytt (+)** och klicka sedan på Tillämpa meddelandekryptering och **rättighetsskydd i Office 365 för meddelanden.**</span><span class="sxs-lookup"><span data-stu-id="a9e6a-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a9e6a-107">Ange **ett** namn på regeln i Namn, till exempel Kryptera meddelanden *som skickas till DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="a9e6a-108">I **Använd den här regeln om** väljer du mottagaren > är den här **personen**.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="a9e6a-109">I fönstret **Välj medlemmar** väljer du namnet på den person som du vill att krypteringsregeln ska gälla för och klickar sedan på lägg **till**.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="a9e6a-110">När du har lagt till alla användare klickar du på **OK.**</span><span class="sxs-lookup"><span data-stu-id="a9e6a-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="a9e6a-111">Klicka på **Markera ett bredvid** Gör följande **fält.**</span><span class="sxs-lookup"><span data-stu-id="a9e6a-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="a9e6a-112">I den **nedrullningsmenyn** för RMS-mallen väljer **du Kryptera** och klickar sedan på **OK.**</span><span class="sxs-lookup"><span data-stu-id="a9e6a-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a9e6a-113">(Om du inte ser det här alternativet innebär det att din plan inte innehåller automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a9e6a-114">Men du kan lägga till den!)</span><span class="sxs-lookup"><span data-stu-id="a9e6a-114">But you can add it!)</span></span>
9. <span data-ttu-id="a9e6a-115">Välj valfritt val (i en lista med valfria val som du kan göra i det här läget. Många av dem kan lämnas med standardinställningen för enkelhetens skull).</span><span class="sxs-lookup"><span data-stu-id="a9e6a-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a9e6a-116">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9e6a-117">Du kan alltid gå tillbaka och redigera regeln senare.</span><span class="sxs-lookup"><span data-stu-id="a9e6a-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a9e6a-118">Mer information om hur du skapar regler för kryptering finns i [Definiera e-postflödesregler för att kryptera e-postmeddelanden i Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a9e6a-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

