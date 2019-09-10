---
title: Flytta e-postmeddelanden till arkivpostlådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822180"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d7c88-102">Flytta e-post till arkivpostlådan</span><span class="sxs-lookup"><span data-stu-id="d7c88-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="d7c88-103">Bekräfta att en **arkivpostlåda** har aktiverats.</span><span class="sxs-lookup"><span data-stu-id="d7c88-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d7c88-104">Om inte, Använd stegen i [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) för att aktivera arkivpostlådan.</span><span class="sxs-lookup"><span data-stu-id="d7c88-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d7c88-105">Om du vill arkivera meddelanden automatiskt till arkivpostlådan måste en kvarhållningstagg med åtgärden **Flytta till Arkiv** vara inställd på **tillämpas automatiskt på hela postlådan (standard)-taggen**.</span><span class="sxs-lookup"><span data-stu-id="d7c88-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d7c88-106">Använd stegen här för att skapa taggen: [Arkiv standard tagg](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="d7c88-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="d7c88-107">Lägg sedan till **arkivtaggen** i din bevarandeprincip.</span><span class="sxs-lookup"><span data-stu-id="d7c88-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d7c88-108">I Exchange administratörscenter, Välj **bevarandeprinciper** > Lägg till **Flytta till arkivtagg** till principen > **Spara**.</span><span class="sxs-lookup"><span data-stu-id="d7c88-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d7c88-109">[Tilldela nu bevarandeprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="d7c88-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d7c88-110">Samma princip kommer att tillämpas på både den **primära** och **arkivera** postlådan.</span><span class="sxs-lookup"><span data-stu-id="d7c88-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d7c88-111">Det kan vara nödvändigt att tvinga assistenten för hanterade mappar (MFA) att köra och tillämpa de nya inställningarna på användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="d7c88-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d7c88-112">Kör följande kommando när du [är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="d7c88-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d7c88-113">Start-ManagedFolderAssistant-identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d7c88-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d7c88-114">Mer information om hur du konfigurerar en arkivprincip finns [i ställa in en Arkiv-och Borttagningsprincip för postlådor](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="d7c88-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  