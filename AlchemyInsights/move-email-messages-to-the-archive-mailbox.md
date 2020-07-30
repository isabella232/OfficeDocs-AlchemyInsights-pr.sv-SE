---
title: Flytta e-postmeddelanden till arkivpostlådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522789"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="57bc7-102">Flytta e-post till arkivpostlådan</span><span class="sxs-lookup"><span data-stu-id="57bc7-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="57bc7-103">Om du vill att vi ska köra automatiska kontroller för de inställningar som nämns nedan, välj bakåtknappen < - högst upp på den här sidan och ange sedan e-postadressen till den användare som har problem med att flytta e-post till sin arkivpostlåda.</span><span class="sxs-lookup"><span data-stu-id="57bc7-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="57bc7-104">Bekräfta att en **arkivpostlåda** har aktiverats.</span><span class="sxs-lookup"><span data-stu-id="57bc7-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="57bc7-105">Om inte, gör du så här i den [här artikeln](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) för att aktivera arkivpostlådan.</span><span class="sxs-lookup"><span data-stu-id="57bc7-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="57bc7-106">Om du vill arkivera meddelanden automatiskt till arkivpostlådan måste en kvarhållningstagg med åtgärden **Flytta till arkiv** ställas in på att tillämpas automatiskt på hela **postlådetaggen (standard)**.</span><span class="sxs-lookup"><span data-stu-id="57bc7-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="57bc7-107">Följ stegen här för att skapa taggen: [Arkiv standardtagg](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="57bc7-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="57bc7-108">Lägg sedan till **arkivtaggen** i bevarandeprincipen.</span><span class="sxs-lookup"><span data-stu-id="57bc7-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="57bc7-109">I administrationscentret för Exchange väljer du **Bevarandeprinciper** > lägga **till taggen Flytta i arkiv** i principen > **Spara**.</span><span class="sxs-lookup"><span data-stu-id="57bc7-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="57bc7-110">Tilldela [nu bevarandeprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="57bc7-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="57bc7-111">Samma princip tillämpas på både **postlådan Primär** och **Arkiv.**</span><span class="sxs-lookup"><span data-stu-id="57bc7-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="57bc7-112">Det kan vara nödvändigt att tvinga MFA (Managed Folder Assistant) att köra och tillämpa de nya inställningarna på användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="57bc7-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="57bc7-113">Kör följande kommando när [du är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="57bc7-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="57bc7-114">Start-ManagedFolderAssistant -Identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="57bc7-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="57bc7-115">Mer information om hur du konfigurerar en arkivprincip finns i [Konfigurera en arkiv- och borttagningsprincip för postlådor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="57bc7-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  