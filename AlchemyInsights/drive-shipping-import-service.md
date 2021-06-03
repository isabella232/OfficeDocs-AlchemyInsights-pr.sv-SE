---
title: Skicka in en hårddisk Microsoft 365 importtjänsten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731949"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="c6874-102">Skicka in en hårddisk Microsoft 365 importtjänsten</span><span class="sxs-lookup"><span data-stu-id="c6874-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="c6874-103">Använd skicka in en hårddisk genom att kopiera PST-filer till en hårddisk och sedan skicka hårddisken till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6874-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="c6874-104">Så här startar du jobbet:</span><span class="sxs-lookup"><span data-stu-id="c6874-104">To start the job:</span></span>

1. <span data-ttu-id="c6874-105">Välj Microsoft 365 i **kompatibilitetscentret** under **Informationsstyrning.**</span><span class="sxs-lookup"><span data-stu-id="c6874-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="c6874-106">Välj **Välj importjobbtyp** och välj sedan **Nästa.**</span><span class="sxs-lookup"><span data-stu-id="c6874-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="c6874-107">För att se stegen för det här importalternativet **väljer du Ship hard drives to one of our physical locations**.</span><span class="sxs-lookup"><span data-stu-id="c6874-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="c6874-108">Här är några saker att tänka på:</span><span class="sxs-lookup"><span data-stu-id="c6874-108">Here are some things to remember:</span></span>

- <span data-ttu-id="c6874-109">Du måste vara tilldelad rollen Importera och exportera postlåda i Exchange Online kunna importera PST-filer till Microsoft 365 postlådor.</span><span class="sxs-lookup"><span data-stu-id="c6874-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="c6874-110">Prestanda kan påverkas för PSTs som är större än 20 GB.</span><span class="sxs-lookup"><span data-stu-id="c6874-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="c6874-111">Endast 2,5-tums SSD (Solid-state Drives) eller 2,5- eller 3,5-tums SATA II/III interna hårddiskar stöds.</span><span class="sxs-lookup"><span data-stu-id="c6874-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="c6874-112">Hårddisken som innehåller PST-filer måste krypteras med BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c6874-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="c6874-113">Kostnaden för att importera PST-filer Microsoft 365 postlådor som använder leverans är 2 USD per GB data.</span><span class="sxs-lookup"><span data-stu-id="c6874-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="c6874-114">Mer information om hur du använder metoden för att skicka in en hårddisk för att importera PST-filer finns i Använda möjligheten att skicka in en hårddisk för [att importera organisationens PST-filer.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="c6874-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>