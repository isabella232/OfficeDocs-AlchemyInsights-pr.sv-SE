---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712202"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0882f-102">DLP kan behöva en anpassad typ</span><span class="sxs-lookup"><span data-stu-id="0882f-102">DLP might need a custom type</span></span>

<span data-ttu-id="0882f-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0882f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0882f-104">**DLP kan kräva en anpassad informations typ**</span><span class="sxs-lookup"><span data-stu-id="0882f-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="0882f-105">Med en policy för att förhindra data förlust (DLP) kan du identifiera och skydda känslig information i organisationen.</span><span class="sxs-lookup"><span data-stu-id="0882f-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0882f-106">I vissa fall kan du behöva skapa en **egen känslig informations** typ för att skydda organisationens data.</span><span class="sxs-lookup"><span data-stu-id="0882f-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0882f-107">Din organisation kan till exempel behöva identifiera och skydda anställnings-ID eller andra data i vissa format som är specifika för din organisation. Om så är fallet, se följande artiklar för mer information.</span><span class="sxs-lookup"><span data-stu-id="0882f-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="0882f-108">**Anpassa en inbyggd typ av känslig information**</span><span class="sxs-lookup"><span data-stu-id="0882f-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0882f-109">Om en inbyggd känslig informations typ uppfyller dina behov med bara några få saker kan du [Anpassa en inbyggd känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0882f-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0882f-110">Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stöd bevis, till exempel ett datum eller en adress.</span><span class="sxs-lookup"><span data-stu-id="0882f-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0882f-111">**Skapa en anpassad känslig informations typ**</span><span class="sxs-lookup"><span data-stu-id="0882f-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0882f-112">Men om du behöver identifiera och skydda en annan typ av känslig information kan du [skapa en anpassad känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i användar gränssnittet för säkerhets & efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="0882f-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="0882f-113">**Skapa en anpassad känslig informations typ i säkerhets & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="0882f-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0882f-114">Om användar gränssnittet inte tillhandahåller alla alternativ du behöver kan du [skapa en anpassad känslig informations typ i säkerhets & kompabilitets Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="0882f-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0882f-115">Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.</span><span class="sxs-lookup"><span data-stu-id="0882f-115">By starting with an XML file, you can use every option available.</span></span>
