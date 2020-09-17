---
title: Flytta e-postmeddelanden till Arkiv post lådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799798"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="1478d-102">Flytta e-post till Arkiv post lådan</span><span class="sxs-lookup"><span data-stu-id="1478d-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="1478d-103">Om du vill att vi ska köra automatisk kontroll för de inställningar som beskrivs nedan, väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för den användare som har problem med att flytta e-post till deras Arkiv post låda.</span><span class="sxs-lookup"><span data-stu-id="1478d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="1478d-104">Bekräfta att en **Arkiv post låda** har Aktiver ATS.</span><span class="sxs-lookup"><span data-stu-id="1478d-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="1478d-105">Om inte, Använd anvisningarna i [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) för att aktivera Arkiv post lådan.</span><span class="sxs-lookup"><span data-stu-id="1478d-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="1478d-106">Om du vill att meddelanden ska arkiveras automatiskt i Arkiv post lådan måste en bevarande tagg med åtgärden **Flytta till Arkiv** -uppgift vara inställd på att **tillämpas automatiskt på hela post låda (standard)**.</span><span class="sxs-lookup"><span data-stu-id="1478d-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="1478d-107">Följ stegen här för att skapa taggen: [arkivera standard märke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="1478d-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="1478d-108">Lägg sedan till **Arkiv** tag gen i bevarande princip.</span><span class="sxs-lookup"><span data-stu-id="1478d-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="1478d-109">I administrations centret för Exchange väljer du **bevarande principer** > lägger till **taggen flytta till Arkiv** till den princip > **Spara**.</span><span class="sxs-lookup"><span data-stu-id="1478d-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="1478d-110">[Tilldela bevarande principen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens post låda.</span><span class="sxs-lookup"><span data-stu-id="1478d-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="1478d-111">Samma policy kommer att tillämpas på både den **primära** och **Arkiv** post lådan.</span><span class="sxs-lookup"><span data-stu-id="1478d-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="1478d-112">Det kan vara nödvändigt att tvinga den Managed mapp Assistant (MFA) att köras och tillämpa de nya inställningarna på användarens post låda.</span><span class="sxs-lookup"><span data-stu-id="1478d-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="1478d-113">Kör följande kommando när du [är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss post låda:</span><span class="sxs-lookup"><span data-stu-id="1478d-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="1478d-114">Start-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="1478d-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="1478d-115">Mer information om hur du konfigurerar en Arkiv princip finns i [Konfigurera en arkiverings-och borttagnings princip för post lådor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="1478d-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  