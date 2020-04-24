---
title: Konfigurera automatiska svar för en postlåda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788900"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="30a11-102">Konfigurera automatiska svar för en användares postlåda</span><span class="sxs-lookup"><span data-stu-id="30a11-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="30a11-103">**Metod 1**</span><span class="sxs-lookup"><span data-stu-id="30a11-103">**Method 1**</span></span>

1. <span data-ttu-id="30a11-104">Logga in på Microsoft 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="30a11-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="30a11-105">Gå till **Användare > Aktiva användare** (eller **Grupper > Delade postlådor** om du konfigurerar detta på en delad postlåda).</span><span class="sxs-lookup"><span data-stu-id="30a11-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="30a11-106">Välj en användare som har en Microsoft Exchange-postlåda.</span><span class="sxs-lookup"><span data-stu-id="30a11-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="30a11-107">I den utfällbara menyn till höger går du till **E-postinställningar > Automatiska svar** (om det är en delad postlåda klickar du på **Automatiska svar** i den utfällbara menyn).</span><span class="sxs-lookup"><span data-stu-id="30a11-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="30a11-108">**Metod 2**</span><span class="sxs-lookup"><span data-stu-id="30a11-108">**Method 2**</span></span>

1. <span data-ttu-id="30a11-109">Logga in på administrationsportalen för Microsoft 365 med administratörens autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="30a11-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="30a11-110">Expandera **Administrationscenter** och klicka sedan på **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="30a11-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="30a11-111">Klicka på bilden i det övre högra hörnet, klicka på **En annan användare** och välj sedan den användarpostlåda som du vill ändra.</span><span class="sxs-lookup"><span data-stu-id="30a11-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="30a11-112">På vänster sida väljer du **Alternativ**, klickar på **Ordna e-post** och sedan på **Automatiska svar.**</span><span class="sxs-lookup"><span data-stu-id="30a11-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="30a11-113">**Metod 3**</span><span class="sxs-lookup"><span data-stu-id="30a11-113">**Method 3**</span></span>

<span data-ttu-id="30a11-114">Kör följande cmdlet i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="30a11-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="30a11-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="30a11-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="30a11-116">Mer information om den här cmdleten finns i [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="30a11-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
