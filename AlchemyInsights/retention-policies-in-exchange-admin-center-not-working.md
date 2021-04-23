---
title: Bevarandeprinciper i administrationscentret för Exchange fungerar inte
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952246"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="65e01-102">Bevarandeprinciper i administrationscentret för Exchange</span><span class="sxs-lookup"><span data-stu-id="65e01-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="65e01-103">Om du vill att vi ska köra automatiska kontroller för inställningarna som nämns nedan väljer du bakåtknappen < – högst upp på den här sidan och anger sedan e-postadressen till den användare som har problem med bevarandeprinciper.</span><span class="sxs-lookup"><span data-stu-id="65e01-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="65e01-104">Om du har problem med bevarandeprinciper i administrationscentret för Exchange som inte gäller för postlådor eller objekt som inte flyttas till arkivpostlådan kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="65e01-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="65e01-105">**Rotorsaker:**</span><span class="sxs-lookup"><span data-stu-id="65e01-105">**Root Causes:**</span></span>

- <span data-ttu-id="65e01-106">**Assistenten för hanterade** mappar har inte bearbetat användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="65e01-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="65e01-107">Assistenten för hanterade mappar försöker att bearbeta alla postlådor i den molnbaserade organisationen en gång var sju:e dag.</span><span class="sxs-lookup"><span data-stu-id="65e01-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="65e01-108">**Lösning:** Kör assistenten för hanterade mappar.</span><span class="sxs-lookup"><span data-stu-id="65e01-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="65e01-109">**RetentionHold** har **aktiverats** för postlådan.</span><span class="sxs-lookup"><span data-stu-id="65e01-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="65e01-110">Om postlådan har placerats på ett RetentionHold bearbetas inte bevarandeprincipen för postlådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="65e01-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="65e01-111">**Lösning:** Kontrollera status för inställningen Bevarande av bevarande och uppdatera efter behov.</span><span class="sxs-lookup"><span data-stu-id="65e01-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="65e01-112">Mer information finns i [Bevarande av postlåda.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="65e01-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="65e01-113">**Obs!** Om en postlåda är mindre än 10 MB bearbetar inte assistenten för hanterade mappar automatiskt postlådan.</span><span class="sxs-lookup"><span data-stu-id="65e01-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="65e01-114">Mer information om bevarandeprinciper i administrationscentret för Exchange finns i:</span><span class="sxs-lookup"><span data-stu-id="65e01-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="65e01-115">Bevarandetaggar och bevarandeprinciper</span><span class="sxs-lookup"><span data-stu-id="65e01-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="65e01-116">[Använda en bevarandeprincip på postlådor eller Lägga](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [till eller ta bort bevarandetaggar](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="65e01-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="65e01-117">Identifiera typen av undantag som tillämpas på en postlåda</span><span class="sxs-lookup"><span data-stu-id="65e01-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
