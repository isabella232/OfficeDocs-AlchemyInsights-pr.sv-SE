---
title: Flera objekt har samma e-postadress som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439709"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="4a01c-102">Flera objekt har samma e-postadress som identitet</span><span class="sxs-lookup"><span data-stu-id="4a01c-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="4a01c-103">**Flera objekt**</span><span class="sxs-lookup"><span data-stu-id="4a01c-103">**Multiple objects**</span></span>

<span data-ttu-id="4a01c-104">En av de vanligaste orsakerna till det här felet är att inte kunna dirigera en Outlook Web Access-begäran korrekt i närvaro av flera objekt som har samma e-postadress som identitet.</span><span class="sxs-lookup"><span data-stu-id="4a01c-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="4a01c-105">Om du vill söka efter dessa objekt kör du följande kommandon:</span><span class="sxs-lookup"><span data-stu-id="4a01c-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="4a01c-106">· Mottagare<email address></span><span class="sxs-lookup"><span data-stu-id="4a01c-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="4a01c-107">· Hämta användare<email address></span><span class="sxs-lookup"><span data-stu-id="4a01c-107">· Get-User <email address></span></span>

<span data-ttu-id="4a01c-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="4a01c-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="4a01c-109">· Få kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="4a01c-109">· Get-Contact <email address></span></span>

<span data-ttu-id="4a01c-110">· Hämta-postlåda <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="4a01c-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="4a01c-111">· Hämta brevlåda <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="4a01c-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="4a01c-112">· Hämta brevlåda <email address> -InaktivaPostlådandå</span><span class="sxs-lookup"><span data-stu-id="4a01c-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="4a01c-113">Lös problemet genom att ta bort flera objekt med samma e-postidentitet och se till att det finns ett enda objekt med den specifika e-postidentiteten och att mottagaren är UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="4a01c-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="4a01c-114">**Samma adress används för företags- och konsumentbrevlådor**</span><span class="sxs-lookup"><span data-stu-id="4a01c-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="4a01c-115">En annan orsak är när samma adress används för företags- och konsumentpostlådor.</span><span class="sxs-lookup"><span data-stu-id="4a01c-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="4a01c-116">I det här fallet måste användaren ändra sitt primära konsumentalias tills Cafe stöder det här scenariot.</span><span class="sxs-lookup"><span data-stu-id="4a01c-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="4a01c-117">Detta är ett permanent fel som inte försvinner utan ingripande.</span><span class="sxs-lookup"><span data-stu-id="4a01c-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="4a01c-118">Mer information finns i [Ändra e-postadressen eller telefonnumret för ditt Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="4a01c-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>