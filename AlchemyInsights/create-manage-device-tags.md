---
title: Skapa och hantera enhetstaggar eller grupper
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
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731969"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="8dbe6-102">Skapa och hantera enhetstaggar eller grupper</span><span class="sxs-lookup"><span data-stu-id="8dbe6-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="8dbe6-103">Lägg till taggar på enheter för att skapa logiskt grupp samarbete.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="8dbe6-104">Enhetstaggar stöder korrekt mappning av nätverket, så att du kan bifoga olika taggar för att fånga sammanhang och möjliggöra skapande av dynamiska listor som en del av ett problem.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="8dbe6-105">Taggar kan användas som ett filter i listvyn Enheter eller för att gruppera enheter.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="8dbe6-106">Mer information om enhetsgruppering finns i Skapa [och hantera enhetstaggar.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="8dbe6-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="8dbe6-107">Du kan lägga till taggar på enheter genom att:</span><span class="sxs-lookup"><span data-stu-id="8dbe6-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="8dbe6-108">Med hjälp av portalen</span><span class="sxs-lookup"><span data-stu-id="8dbe6-108">Using the portal</span></span>

- <span data-ttu-id="8dbe6-109">Ange ett registernyckelvärde</span><span class="sxs-lookup"><span data-stu-id="8dbe6-109">Setting a registry key value</span></span>
 
<span data-ttu-id="8dbe6-110">**Obs!** Det kan finnas fördröjning mellan tiden då en tagg läggs till på en enhet och dess tillgänglighet i listan över enheter och på sidan enhet.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="8dbe6-111">Information om hur du lägger till enhetstaggar med API finns [i Lägga till eller ta bort API för enhetstaggar.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="8dbe6-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="8dbe6-112">Lägga till och hantera enhetstaggar via portalen</span><span class="sxs-lookup"><span data-stu-id="8dbe6-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="8dbe6-113">Välj den enhet där du vill hantera taggar.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="8dbe6-114">Du kan välja eller söka efter en enhet i någon av följande vyer:</span><span class="sxs-lookup"><span data-stu-id="8dbe6-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="8dbe6-115">**Instrumentpanel för säkerhetsåtgärder** Välj enhetens namn i avsnittet Populära enheter med aktiva aviseringar.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="8dbe6-116">**Telefonaviseringar** – Välj enhetsnamnet bredvid enhetsikonen från aviseringskön.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="8dbe6-117">**Listan Enheter** – Välj enhetsnamnet i listan över enheter.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="8dbe6-118">**Sökruta** – Välj enhet i listrutan och ange enhetens namn.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="8dbe6-119">Du kan också gå till aviseringssidan via filen och IP-vyerna.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="8dbe6-120">Välj **Hantera taggar** i raden med svarsåtgärder.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="8dbe6-121">Skriv för att hitta eller skapa taggar.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-121">Type to find or create tags.</span></span>

<span data-ttu-id="8dbe6-122">Taggar läggs till i enhetsvyn och visas i listvyn Enheter.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="8dbe6-123">Sedan kan du använda filtret Taggar för att se den relevanta listan över enheter.</span><span class="sxs-lookup"><span data-stu-id="8dbe6-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="8dbe6-124">Mer information finns i Skapa [och hantera enhetstaggar.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="8dbe6-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>