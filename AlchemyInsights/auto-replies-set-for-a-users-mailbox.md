---
title: Konfigurera automatiska svar för en postlåda
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820952"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="2c0b6-102">Konfigurera automatiska svar för en användares postlåda</span><span class="sxs-lookup"><span data-stu-id="2c0b6-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="2c0b6-103">**Metod 1**</span><span class="sxs-lookup"><span data-stu-id="2c0b6-103">**Method 1**</span></span>

1. <span data-ttu-id="2c0b6-104">Logga in på Microsoft 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="2c0b6-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="2c0b6-105">Gå till **Användare > Aktiva användare** (eller **Grupper > Delade postlådor** om du konfigurerar detta på en delad postlåda).</span><span class="sxs-lookup"><span data-stu-id="2c0b6-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="2c0b6-106">Välj en användare som har en Microsoft Exchange-postlåda.</span><span class="sxs-lookup"><span data-stu-id="2c0b6-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="2c0b6-107">I den utfällbara menyn till höger går du till **E-postinställningar > Automatiska svar** (om det är en delad postlåda klickar du på **Automatiska svar** i den utfällbara menyn).</span><span class="sxs-lookup"><span data-stu-id="2c0b6-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="2c0b6-108">**Metod 2**</span><span class="sxs-lookup"><span data-stu-id="2c0b6-108">**Method 2**</span></span>

1. <span data-ttu-id="2c0b6-109">Logga in på administrationsportalen för Microsoft 365 med administratörens autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="2c0b6-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="2c0b6-110">Expandera **Administrationscenter** och klicka sedan på **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2c0b6-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="2c0b6-111">Klicka på bilden i det övre högra hörnet, klicka på **En annan användare** och välj sedan den användarpostlåda som du vill ändra.</span><span class="sxs-lookup"><span data-stu-id="2c0b6-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="2c0b6-112">På vänster sida väljer du **Alternativ**, klickar på **Ordna e-post** och sedan på **Automatiska svar.**</span><span class="sxs-lookup"><span data-stu-id="2c0b6-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="2c0b6-113">**Metod 3**</span><span class="sxs-lookup"><span data-stu-id="2c0b6-113">**Method 3**</span></span>

<span data-ttu-id="2c0b6-114">Kör följande cmdlet i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2c0b6-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="2c0b6-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="2c0b6-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="2c0b6-116">Mer information om den här cmdleten finns i [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="2c0b6-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
