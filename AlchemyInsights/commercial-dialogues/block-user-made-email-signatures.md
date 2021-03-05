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
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483364"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="60fed-102">Blockera användarbaserade e-postsignaturer</span><span class="sxs-lookup"><span data-stu-id="60fed-102">Block user-made email signatures</span></span>

<span data-ttu-id="60fed-103">Följande lösning gäller endast för e-postsignaturer som skapas i Outlook på webben.</span><span class="sxs-lookup"><span data-stu-id="60fed-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="60fed-104">Du kan bara blockera signaturer i Outlook-appen om du har en lokal Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="60fed-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="60fed-105">Välj Administrationscenter för Exchange i  >  **administrationscentret.**</span><span class="sxs-lookup"><span data-stu-id="60fed-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="60fed-106">Klicka **på behörigheter** för Outlook Web  >  **App-principer.**</span><span class="sxs-lookup"><span data-stu-id="60fed-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="60fed-107">Markera principen och klicka sedan på pennikonen för att redigera den.</span><span class="sxs-lookup"><span data-stu-id="60fed-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="60fed-108">Klicka **på fler** alternativ för  >  **funktioner.**</span><span class="sxs-lookup"><span data-stu-id="60fed-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="60fed-109">Avmarkera kryssrutan E-postsignatur **under** Användarupplevelse och klicka sedan på **Spara.** </span><span class="sxs-lookup"><span data-stu-id="60fed-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="60fed-110">**Viktigt:** Om en signatur har lagts till innan du avmarkerar den här kryssrutan kan användaren fortfarande använda den.</span><span class="sxs-lookup"><span data-stu-id="60fed-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="60fed-111">Be dem att ta bort den.</span><span class="sxs-lookup"><span data-stu-id="60fed-111">Ask them to remove it.</span></span>
