---
title: Söka efter adresser för vidarebefordran i postlådor
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403329"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="2d2c1-102">Söka efter adresser för vidarebefordran i postlådor</span><span class="sxs-lookup"><span data-stu-id="2d2c1-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="2d2c1-103">Ibland kan hackare vidarebefordra användarnas e-postmeddelanden till sig själva, så först ska vi kontrollera om det finns adresser och regler för vidarebefordran av postlådan.</span><span class="sxs-lookup"><span data-stu-id="2d2c1-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="2d2c1-104">Sedan kontrollerar vi granskningsloggarna.</span><span class="sxs-lookup"><span data-stu-id="2d2c1-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="2d2c1-105">Så här kontrollerar du om det finns adresser för vidarebefordran:</span><span class="sxs-lookup"><span data-stu-id="2d2c1-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="2d2c1-106">Välj **Användare**  >  **Aktiva användare.**</span><span class="sxs-lookup"><span data-stu-id="2d2c1-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="2d2c1-107">Välj den användare vars konto har komprometterats.</span><span class="sxs-lookup"><span data-stu-id="2d2c1-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="2d2c1-108">I den utfällmapp som visas expanderar du **E-postinställningar** och klickar sedan **på Redigera under** **Vidarebefordran av e-post.**</span><span class="sxs-lookup"><span data-stu-id="2d2c1-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="2d2c1-109">Ta bort alla adresser för vidarebefordran som du inte känner igen.</span><span class="sxs-lookup"><span data-stu-id="2d2c1-109">Remove any forwarding addresses you don't recognize.</span></span>