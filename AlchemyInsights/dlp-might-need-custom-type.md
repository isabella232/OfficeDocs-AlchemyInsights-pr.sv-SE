---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932676"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6d376-102">DLP kan behöva en anpassad typ</span><span class="sxs-lookup"><span data-stu-id="6d376-102">DLP might need a custom type</span></span>

<span data-ttu-id="6d376-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="6d376-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6d376-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="6d376-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6d376-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="6d376-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6d376-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="6d376-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6d376-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="6d376-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6d376-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="6d376-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6d376-109">**DLP kan kräva en anpassad informationstyp**</span><span class="sxs-lookup"><span data-stu-id="6d376-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="6d376-110">Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen.</span><span class="sxs-lookup"><span data-stu-id="6d376-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6d376-111">I vissa fall kan du behöva skapa en egen **anpassad** känslig informationstyp för att skydda organisationens data.</span><span class="sxs-lookup"><span data-stu-id="6d376-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6d376-112">Din organisation kan till exempel behöva identifiera och skydda medarbetar-ID:er eller andra data i något format som är specifikt för din organisation. Om så är fallet, se följande artiklar för mer information.</span><span class="sxs-lookup"><span data-stu-id="6d376-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="6d376-113">**Anpassa en inbyggd känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="6d376-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6d376-114">Om en inbyggd känslig informationstyp skulle uppfylla dina behov med bara några justeringar, kan du [anpassa en inbyggd känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6d376-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6d376-115">Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.</span><span class="sxs-lookup"><span data-stu-id="6d376-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6d376-116">**Skapa en anpassad känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="6d376-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6d376-117">Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du [skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i användargränssnittet i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="6d376-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="6d376-118">**Skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="6d376-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6d376-119">Om användargränssnittet inte innehåller alla alternativ du behöver kan du [slutligen skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6d376-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6d376-120">Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.</span><span class="sxs-lookup"><span data-stu-id="6d376-120">By starting with an XML file, you can use every option available.</span></span>
