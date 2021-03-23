---
title: Importera och exportera från Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037257"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="c8411-102">Importera och exportera från Yammer</span><span class="sxs-lookup"><span data-stu-id="c8411-102">Import and export from Yammer</span></span>

<span data-ttu-id="c8411-103">**Importera**</span><span class="sxs-lookup"><span data-stu-id="c8411-103">**Import**</span></span>

<span data-ttu-id="c8411-104">Alternativen för användarimport varierar beroende på om Yammer-nätverket är i [inbyggt läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller inte.</span><span class="sxs-lookup"><span data-stu-id="c8411-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="c8411-105">**Icke-inbyggt läge:** Användare kan importeras till grupper med hjälp av Lägg till från adressbok [(begränsning](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) till 100 användare) i gruppinställningar eller i nätverket med [Massuppdatering](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) inom nätverksadministratören.</span><span class="sxs-lookup"><span data-stu-id="c8411-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="c8411-106">**Inbyggt läge:** Åtgärder för gruppmedlemskap och nätverksmedlemskap ska utföras från [Microsoft 365-administratörsportalen,](https://docs.microsoft.com/microsoft-365/admin/add-users)Azure [AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ett annat Azure AD-alternativ.</span><span class="sxs-lookup"><span data-stu-id="c8411-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="c8411-107">Nätverk i inbyggt läge har inte längre tillgång till Massuppdatering och andra äldre funktioner.</span><span class="sxs-lookup"><span data-stu-id="c8411-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8411-108">Yammer hade aldrig stöd för import av innehåll från nätverksadministratören även när funktionen Dataexport användes i ett annat nätverk.</span><span class="sxs-lookup"><span data-stu-id="c8411-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="c8411-109">Innehåll kan publiceras på nytt av partnerlösningar eller REST-API:er för Yammer.</span><span class="sxs-lookup"><span data-stu-id="c8411-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="c8411-110">**Exportera**</span><span class="sxs-lookup"><span data-stu-id="c8411-110">**Export**</span></span>

<span data-ttu-id="c8411-111">[Exportera nätverksdata inom nätverksadministratören](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillåter export av innehåll från Yammer-nätverk, inklusive meddelanden och filer.</span><span class="sxs-lookup"><span data-stu-id="c8411-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="c8411-112">Bifogade filer kan vara extremt stora och exporter tar lång tid att slutföra.</span><span class="sxs-lookup"><span data-stu-id="c8411-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="c8411-113">Vi rekommenderar att aktiva nätverk exporteras med API:t [för dataexport](https://developer.yammer.com/docs/data-export-api) i delar per dag eller vecka.</span><span class="sxs-lookup"><span data-stu-id="c8411-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="c8411-114">Microsoft Support tillhandahåller inte egna skript för detta ändamål.</span><span class="sxs-lookup"><span data-stu-id="c8411-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="c8411-115">Det finns [en separat GDPR-export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) för att exportera innehåll för en enskild användare.</span><span class="sxs-lookup"><span data-stu-id="c8411-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>