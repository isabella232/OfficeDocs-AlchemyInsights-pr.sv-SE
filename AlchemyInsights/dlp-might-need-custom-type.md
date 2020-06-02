---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507532"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2f76c-102">DLP kan behöva en anpassad typ</span><span class="sxs-lookup"><span data-stu-id="2f76c-102">DLP might need a custom type</span></span>

<span data-ttu-id="2f76c-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2f76c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2f76c-104">**DLP kan kräva en anpassad informationstyp**</span><span class="sxs-lookup"><span data-stu-id="2f76c-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2f76c-105">Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen.</span><span class="sxs-lookup"><span data-stu-id="2f76c-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2f76c-106">I vissa fall kan du behöva skapa en egen **anpassad** känslig informationstyp för att skydda organisationens data.</span><span class="sxs-lookup"><span data-stu-id="2f76c-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2f76c-107">Din organisation kan till exempel behöva identifiera och skydda medarbetar-ID:er eller andra data i något format som är specifikt för din organisation. Om så är fallet, se följande artiklar för mer information.</span><span class="sxs-lookup"><span data-stu-id="2f76c-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2f76c-108">**Anpassa en inbyggd känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="2f76c-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2f76c-109">Om en inbyggd känslig informationstyp skulle uppfylla dina behov med bara några justeringar, kan du [anpassa en inbyggd känslig informationstyp](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2f76c-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2f76c-110">Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.</span><span class="sxs-lookup"><span data-stu-id="2f76c-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2f76c-111">**Skapa en anpassad känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="2f76c-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2f76c-112">Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du [skapa en anpassad känslig informationstyp](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i användargränssnittet i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="2f76c-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2f76c-113">**Skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="2f76c-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2f76c-114">Om användargränssnittet inte innehåller alla alternativ du behöver kan du [slutligen skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2f76c-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2f76c-115">Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.</span><span class="sxs-lookup"><span data-stu-id="2f76c-115">By starting with an XML file, you can use every option available.</span></span>
