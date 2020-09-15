---
title: DLP fungerar inte som förväntat
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679711"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="8f5ce-102">DLP fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="8f5ce-102">DLP not working as expected</span></span>

<span data-ttu-id="8f5ce-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="8f5ce-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="8f5ce-104">**Konfigurera DLP**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-104">**Setting up DLP**</span></span>

<span data-ttu-id="8f5ce-105">Har du problem med **data förlust (DLP)** i Office 365 inte fungerar som det ska?</span><span class="sxs-lookup"><span data-stu-id="8f5ce-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="8f5ce-106">Om så är fallet, se till att **DLP-principen** är korrekt konfigurerad och att dina data innehåller den information som används för att använda DLP- **principen** när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="8f5ce-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="8f5ce-107">Med DLP-principer kan du identifiera och skydda känslig information i organisationen.</span><span class="sxs-lookup"><span data-stu-id="8f5ce-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="8f5ce-108">Använd informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)för att konfigurera DLP-principer.</span><span class="sxs-lookup"><span data-stu-id="8f5ce-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="8f5ce-109">**Vilka DLP-principer som ska sökas efter**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="8f5ce-110">När du använder de **inbyggda känsliga informations typerna** i säkerhets-och EFTERLEVNADSPRINCIPER kan DLP-principer leta efter specifika mönster och element när de här känsliga typerna identifieras.</span><span class="sxs-lookup"><span data-stu-id="8f5ce-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="8f5ce-111">**Inbyggda känsliga informations typer**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="8f5ce-112">Information om de inbyggda känsliga typerna och vilken DLP-princip som används för att identifiera den känsliga typen finns i: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="8f5ce-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="8f5ce-113">**Anpassade typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="8f5ce-114">Om du försöker skapa anpassade informations typer kan du använda följande artikel för att få information om hur du skapar en anpassad känslig typ: [skapa en anpassad känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8f5ce-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="8f5ce-115">**Testa en DLP-princip**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-115">**Test a DLP policy**</span></span>

<span data-ttu-id="8f5ce-116">Om du vill testa dina data med en inbyggd eller anpassad känslig informations typ använder du alternativet **testtyp** under **klassificerings**  >  **känsliga informations typer**.</span><span class="sxs-lookup"><span data-stu-id="8f5ce-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="8f5ce-117">Mer information finns i [testa anpassade typer av känslig information](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="8f5ce-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="8f5ce-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="8f5ce-118">**Reports**</span></span>
  
- <span data-ttu-id="8f5ce-119">Få känsliga data insikter med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="8f5ce-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="8f5ce-120">Visa detaljerad information om händelsen med en [incident rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="8f5ce-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
