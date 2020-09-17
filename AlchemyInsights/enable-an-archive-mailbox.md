---
title: Aktivera en Arkiv post låda
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811724"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="5065b-102">Aktivera en Arkiv post låda</span><span class="sxs-lookup"><span data-stu-id="5065b-102">Enable an archive mailbox</span></span>

<span data-ttu-id="5065b-103">Om du vill att vi ska köra automatisk kontroll för att kontrol lera att en Arkiv post låda kan konfigureras väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för kontot.</span><span class="sxs-lookup"><span data-stu-id="5065b-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="5065b-104">Arkiv post lådor i Microsoft 365 (kallas även *online-arkiv* eller *Arkiv på plats*) ger användarna ytterligare e-postlagring.</span><span class="sxs-lookup"><span data-stu-id="5065b-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="5065b-105">Användare kan flytta eller kopiera objekt till deras Arkiv post låda och administratörer kan skapa en princip som automatiskt flyttar objekt till Arkiv post lådor.</span><span class="sxs-lookup"><span data-stu-id="5065b-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="5065b-106">Så här skapar du en Arkiv post låda:</span><span class="sxs-lookup"><span data-stu-id="5065b-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="5065b-107">Gå till [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="5065b-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="5065b-108">Logga in på Microsoft 365 med ditt administratörs konto.</span><span class="sxs-lookup"><span data-stu-id="5065b-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="5065b-109">I det vänstra fönstret i säkerhetsfunktions &amp; Center väljer du **informations** styr \> **Arkiv**.</span><span class="sxs-lookup"><span data-stu-id="5065b-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="5065b-110">Välj den användare vars Arkiv post låda du vill aktivera.</span><span class="sxs-lookup"><span data-stu-id="5065b-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="5065b-111">I informations fönstret till höger klickar du på **Aktivera** och sedan på **Ja** i varnings meddelandet för att aktivera Arkiv post lådan.</span><span class="sxs-lookup"><span data-stu-id="5065b-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="5065b-112">Du kan också aktivera Arkiv post lådor genom att välja flera användare (med **SKIFT** -eller **CTRL** -tangenten) och sedan klicka på **Aktivera** i informations fönstret.</span><span class="sxs-lookup"><span data-stu-id="5065b-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="5065b-113">Delade postlådor</span><span class="sxs-lookup"><span data-stu-id="5065b-113">Shared mailboxes</span></span>

<span data-ttu-id="5065b-114">Om du vill aktivera arkivet för en delad post låda måste du ha en licens för Exchange Online abonnemang 2 eller en Exchange Online plan 1-licens med en Exchange Online-licens.</span><span class="sxs-lookup"><span data-stu-id="5065b-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="5065b-115">Så här aktiverar du arkivet för en delad post låda:</span><span class="sxs-lookup"><span data-stu-id="5065b-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="5065b-116">Gå till [administrations centret för Exchange](https://outlook.office365.com/ecp) och logga in med ditt administratörs konto.</span><span class="sxs-lookup"><span data-stu-id="5065b-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="5065b-117">Gå till **mottagare**som  >  **delas**.</span><span class="sxs-lookup"><span data-stu-id="5065b-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="5065b-118">Välj den delade post lådan.</span><span class="sxs-lookup"><span data-stu-id="5065b-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="5065b-119">I informations fönstret till höger under **Arkiv på plats**klickar du på **Aktivera**och sedan på **Ja** för att aktivera Arkiv post lådan.</span><span class="sxs-lookup"><span data-stu-id="5065b-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="5065b-120">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="5065b-120">For more information, see:</span></span>
  
- [<span data-ttu-id="5065b-121">Aktivera arkivpostlådor</span><span class="sxs-lookup"><span data-stu-id="5065b-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="5065b-122">Konfigurera en princip för arkivering och borttagning</span><span class="sxs-lookup"><span data-stu-id="5065b-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
