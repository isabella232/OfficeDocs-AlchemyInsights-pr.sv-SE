---
title: Automatiskt flytta e-postmeddelanden till arkivpostlådan
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749290"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="97014-102">Automatiskt flytta e-postmeddelanden till arkivpostlådan</span><span class="sxs-lookup"><span data-stu-id="97014-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="97014-103">Så här skapar du en princip för att automatiskt flytta en användares gamla e-post till arkivpostlådan:</span><span class="sxs-lookup"><span data-stu-id="97014-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="97014-104">Gå till [**Säkerhet & för**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **efterlevnadsdatastyrning**  >  **för** att verifiera att en arkivpostlåda har aktiverats för användaren.</span><span class="sxs-lookup"><span data-stu-id="97014-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="97014-105">Om det inte har gjort det klickar **du på** Aktivera **och sedan** Ja i varningsrutan.</span><span class="sxs-lookup"><span data-stu-id="97014-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="97014-106">Gå till [**Exchange admin center > för efterlevnadshantering > bevarandetaggar**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="97014-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="97014-107">Välj ikonen + och välj sedan **automatiskt tillämpas på hela postlådan.**</span><span class="sxs-lookup"><span data-stu-id="97014-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="97014-108">Tilldela bevarandetaggen ett namn och välj **Flytta till arkiv.**</span><span class="sxs-lookup"><span data-stu-id="97014-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="97014-109">Ange hur lång tid du vill ha kvarhållningstiden, till exempel 90 dagar.</span><span class="sxs-lookup"><span data-stu-id="97014-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="97014-110">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="97014-110">Click **Save**.</span></span>
5. <span data-ttu-id="97014-111">Skapa nu en bevarandeprincip: välj **bevarandeprinciper** och välj ikonen för att lägga till en ny princip.</span><span class="sxs-lookup"><span data-stu-id="97014-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="97014-112">Ge bevarandeprincipen ett namn och klicka sedan på och bläddra för att hitta och lägga till den bevarandetagg du just skapade.</span><span class="sxs-lookup"><span data-stu-id="97014-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="97014-113">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="97014-113">Click **Save**.</span></span>
7. <span data-ttu-id="97014-114">Tillämpa slutligen kvarhållningsprincipen på användarens postlåda: gå till mottagarnas postlådor i administrationscentret  >  **för** Exchange.</span><span class="sxs-lookup"><span data-stu-id="97014-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="97014-115">Välj alla användare som du vill tillämpa principen på och välj sedan **Redigera** (pennikonen).</span><span class="sxs-lookup"><span data-stu-id="97014-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="97014-116">Klicka på postlådefunktioner **i dialogrutan.**</span><span class="sxs-lookup"><span data-stu-id="97014-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="97014-117">Tillämpa **den princip** som du just skapade när du > Spara under **Bevarandeprincip.**</span><span class="sxs-lookup"><span data-stu-id="97014-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="97014-118">Instruktioner för hur du tillämpar principen på alla användare finns i [Använda en bevarandeprincip för postlådor.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="97014-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>