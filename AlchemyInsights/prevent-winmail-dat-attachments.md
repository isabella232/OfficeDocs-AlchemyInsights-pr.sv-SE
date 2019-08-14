---
title: 2589 förhindra att bifogade Winmail.dat-filer i e-postmeddelanden från din organisation
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391563"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="38e31-102">Förhindra att Winmail.dat-bilagor i e-postmeddelanden från din organisation</span><span class="sxs-lookup"><span data-stu-id="38e31-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="38e31-103">Prova dessa steg som en administratör:</span><span class="sxs-lookup"><span data-stu-id="38e31-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="38e31-104">Öppna [Exchange administratörscenter](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="38e31-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="38e31-105">Gå till **e-postflödet** > **fjärrdomäner**.</span><span class="sxs-lookup"><span data-stu-id="38e31-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="38e31-106">Välj standard fjärrdomänen med namnet **standard**och klicka sedan på **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="38e31-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="38e31-107">Markera **aldrig**i avsnittet **använda RTF - format** .</span><span class="sxs-lookup"><span data-stu-id="38e31-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="38e31-108">Mer information finns i [Ange meddelandeformatet för fjärrdomäner](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="38e31-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
