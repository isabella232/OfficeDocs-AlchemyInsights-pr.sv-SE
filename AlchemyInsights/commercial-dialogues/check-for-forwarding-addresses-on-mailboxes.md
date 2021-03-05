---
title: Söka efter adresser för vidarebefordran av postlådor
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483925"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c753c-102">Söka efter adresser för vidarebefordran av postlådor</span><span class="sxs-lookup"><span data-stu-id="c753c-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c753c-103">Ibland kan hackare vidarebefordra användarnas e-postmeddelanden till sig själva, så först ska vi kontrollera vidarebefordran av adresser och regler för postlådan.</span><span class="sxs-lookup"><span data-stu-id="c753c-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c753c-104">Sedan kontrollerar vi granskningsloggarna.</span><span class="sxs-lookup"><span data-stu-id="c753c-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c753c-105">Så här kontrollerar du om det finns adresser för vidarebefordran:</span><span class="sxs-lookup"><span data-stu-id="c753c-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c753c-106">Välj **Aktiva**  >  **användare.**</span><span class="sxs-lookup"><span data-stu-id="c753c-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c753c-107">Välj den användare vars konto har komprometterats.</span><span class="sxs-lookup"><span data-stu-id="c753c-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c753c-108">I den utfällmapp som visas expanderar du **E-postinställningar** och klickar sedan **på** Redigera för vidarebefordran **av e-post.**</span><span class="sxs-lookup"><span data-stu-id="c753c-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c753c-109">Ta bort alla adresser för vidarebefordran som du inte känner igen.</span><span class="sxs-lookup"><span data-stu-id="c753c-109">Remove any forwarding addresses you don't recognize.</span></span>