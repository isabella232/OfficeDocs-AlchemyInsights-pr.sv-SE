---
title: Blockera användarbaserade e-postsignaturer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243636"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="fc2c4-102">Blockera användarbaserade e-postsignaturer</span><span class="sxs-lookup"><span data-stu-id="fc2c4-102">Block user-made email signatures</span></span>

<span data-ttu-id="fc2c4-103">Följande lösning gäller endast för e-postsignaturer som skapas i Outlook på webben.</span><span class="sxs-lookup"><span data-stu-id="fc2c4-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="fc2c4-104">Du kan bara blockera signaturer i Outlook-appen om du har en lokal Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="fc2c4-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="fc2c4-105">Välj Administrationscenter för Exchange i  >  **administrationscentret.**</span><span class="sxs-lookup"><span data-stu-id="fc2c4-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="fc2c4-106">Klicka **på behörigheter** för Outlook Web  >  **App-principer.**</span><span class="sxs-lookup"><span data-stu-id="fc2c4-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="fc2c4-107">Markera principen och klicka sedan på pennikonen för att redigera den.</span><span class="sxs-lookup"><span data-stu-id="fc2c4-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="fc2c4-108">Klicka **på fler** alternativ för  >  **funktioner.**</span><span class="sxs-lookup"><span data-stu-id="fc2c4-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="fc2c4-109">Avmarkera kryssrutan E-postsignatur **under** Användarupplevelse och klicka sedan på **Spara.** </span><span class="sxs-lookup"><span data-stu-id="fc2c4-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="fc2c4-110">**Viktigt:** Om en signatur har lagts till innan du avmarkerar den här kryssrutan kan användaren fortfarande använda den.</span><span class="sxs-lookup"><span data-stu-id="fc2c4-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="fc2c4-111">Be dem att ta bort den.</span><span class="sxs-lookup"><span data-stu-id="fc2c4-111">Ask them to remove it.</span></span>
