---
title: Exempel på princip för Säker bifogad fil i Microsoft Defender för Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695187"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="0f617-102">Exempel på princip för Säker bifogad fil i Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="0f617-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="0f617-103">De här inställningarna aktiverar principen *Inga fördröjningar* som levererar meddelanden omedelbart och sedan bifogar bifogade filer igen när de skannas:</span><span class="sxs-lookup"><span data-stu-id="0f617-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="0f617-104">**Namn:** Inga fördröjningar</span><span class="sxs-lookup"><span data-stu-id="0f617-104">**Name**: No delays</span></span>
- <span data-ttu-id="0f617-105">**Beskrivning:** Levererar meddelanden omedelbart och bifogar bifogade filer igen efter genomsökning.</span><span class="sxs-lookup"><span data-stu-id="0f617-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="0f617-106">**Svar:** Välj **alternativet Dynamisk** leverans.</span><span class="sxs-lookup"><span data-stu-id="0f617-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="0f617-107">Mer information finns i principer [för dynamisk leverans i principer för säkra bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="0f617-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="0f617-108">**Avsnittet Omdirigering** av bifogade filer: Välj alternativet för att aktivera omdirigering och ange sedan e-postadressen till din globala Microsoft 365-administratör, säkerhetsadministratör eller säkerhetsanalytiker som undersöker skadliga bifogade filer.</span><span class="sxs-lookup"><span data-stu-id="0f617-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="0f617-109">**Avsnittet Tillämpas** på: **Välj mottagarens domän** är, och välj sedan din domän.</span><span class="sxs-lookup"><span data-stu-id="0f617-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="0f617-110">Välj **Lägg till** och välj sedan **OK.**</span><span class="sxs-lookup"><span data-stu-id="0f617-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="0f617-111">Välj Spara när du är **klar.**</span><span class="sxs-lookup"><span data-stu-id="0f617-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="0f617-112">Mer information finns i Säkra [bifogade filer i Microsoft Defender för Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="0f617-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
