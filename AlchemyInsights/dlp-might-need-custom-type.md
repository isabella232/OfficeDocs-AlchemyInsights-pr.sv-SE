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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052919"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8cf52-102">DLP kan behöva en anpassad typ</span><span class="sxs-lookup"><span data-stu-id="8cf52-102">DLP might need a custom type</span></span>

<span data-ttu-id="8cf52-103">Med en princip för dataförlustskydd (DLP) kan du identifiera och skydda känsliga data i din organisation.</span><span class="sxs-lookup"><span data-stu-id="8cf52-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8cf52-104">I vissa fall kan du behöva skapa en egen **anpassad** känslig informationstyp för att skydda organisationens data.</span><span class="sxs-lookup"><span data-stu-id="8cf52-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8cf52-105">Din organisation kan till exempel behöva identifiera och skydda medarbetar-ID eller andra data i vissa format som är specifika för din org. I så fall finns i följande artiklar för mer information.</span><span class="sxs-lookup"><span data-stu-id="8cf52-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8cf52-106">**Anpassa en inbyggd känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="8cf52-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8cf52-107">Om en inbyggd känslig informationstyp uppfyller dina behov med bara några få tweaks, kan du [Anpassa en inbyggd känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8cf52-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8cf52-108">Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödjande bevis, till exempel ett datum eller en adress.</span><span class="sxs-lookup"><span data-stu-id="8cf52-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8cf52-109">**Skapa en anpassad känslig informationstyp**</span><span class="sxs-lookup"><span data-stu-id="8cf52-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8cf52-110">Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet, kan du [skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i användargränssnittet för säkerhets & Efterlevnadscenter.</span><span class="sxs-lookup"><span data-stu-id="8cf52-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8cf52-111">**Skapa en anpassad känslig informationstyp i Security & Efterlevnadscenter PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8cf52-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8cf52-112">Slutligen, om ANVÄNDARGRÄNSSNITTET inte innehåller alla alternativ som du behöver, kan du [skapa en anpassad känslig informationstyp i Security & Efterlevnadscenter PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="8cf52-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8cf52-113">Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.</span><span class="sxs-lookup"><span data-stu-id="8cf52-113">By starting with an XML file, you can use every option available.</span></span>
