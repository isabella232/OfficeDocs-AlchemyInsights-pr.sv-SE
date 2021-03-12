---
title: Exempel på princip för säkra bifogade filer i Microsoft Defender för Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749195"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="bec6e-102">Exempel på princip för säkra bifogade filer i Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="bec6e-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="bec6e-103">De här inställningarna aktiverar principen *No delays* (Inga fördröjningar) som skickar meddelanden direkt och sedan återansluter bifogade filer när de har skannats:</span><span class="sxs-lookup"><span data-stu-id="bec6e-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="bec6e-104">**Namn**: Inga fördröjningar</span><span class="sxs-lookup"><span data-stu-id="bec6e-104">**Name**: No delays</span></span>
- <span data-ttu-id="bec6e-105">**Beskrivning**: Levererar meddelanden omedelbart ochbibiar bifogade filer efter genomsökning.</span><span class="sxs-lookup"><span data-stu-id="bec6e-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="bec6e-106">**Svar:** Välj **alternativet Dynamisk** leverans.</span><span class="sxs-lookup"><span data-stu-id="bec6e-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="bec6e-107">Mer information finns i Principer [för dynamisk leverans i säkra bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="bec6e-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="bec6e-108">**Avsnittet Omdirigera bifogad** fil: Välj alternativet Aktivera omdirigering och ange sedan e-postadressen till din globala Microsoft 365-administratör, säkerhetsadministratör eller säkerhetsanalytiker som ska undersöka skadliga bifogade filer. </span><span class="sxs-lookup"><span data-stu-id="bec6e-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="bec6e-109">**Avsnittet Används** för: **Välj Mottagarens domän är** och välj sedan din domän.</span><span class="sxs-lookup"><span data-stu-id="bec6e-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="bec6e-110">Välj **lägg** till och välj sedan **OK.**</span><span class="sxs-lookup"><span data-stu-id="bec6e-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="bec6e-111">Välj Spara när du är **klar.**</span><span class="sxs-lookup"><span data-stu-id="bec6e-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="bec6e-112">Mer information finns i Säkra [bifogade filer i Microsoft Defender för Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="bec6e-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
