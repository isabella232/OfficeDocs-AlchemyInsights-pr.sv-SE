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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707828"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="91514-102">DLP fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="91514-102">DLP not working as expected</span></span>

<span data-ttu-id="91514-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="91514-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="91514-104">**Konfigurera DLP**</span><span class="sxs-lookup"><span data-stu-id="91514-104">**Setting up DLP**</span></span>

<span data-ttu-id="91514-105">Fungerar du inte som **förväntat med DLP (Data Loss Prevention)** i Office 365?</span><span class="sxs-lookup"><span data-stu-id="91514-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="91514-106">I så fall kontrollerar du att **DLP-principen** är korrekt konfigurerad och att dina data innehåller det **som DLP-principen** letar efter när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="91514-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="91514-107">Med DLP-principer kan du identifiera och skydda känslig information i organisationen.</span><span class="sxs-lookup"><span data-stu-id="91514-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="91514-108">Om du vill konfigurera DLP-principer använder du informationen [här.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="91514-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="91514-109">**Vad DLP-principer söker efter**</span><span class="sxs-lookup"><span data-stu-id="91514-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="91514-110">När du använder de inbyggda typerna för känslig information i Center för säkerhet och efterlevnad söker **DLP-principerna** efter specifika mönster och element när dessa känsliga typer identifieras.</span><span class="sxs-lookup"><span data-stu-id="91514-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="91514-111">**Inbyggda typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="91514-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="91514-112">Mer information om inbyggda typer av känslig information och vad en DLP-princip söker efter när typen Känslig identifieras finns i: Vilka typer av [känslig information letar du efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="91514-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="91514-113">**Anpassade typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="91514-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="91514-114">Om du vill skapa anpassade typer av känslig information kan du använda följande artikel för information om hur du skapar en anpassad typ av känslig information: Skapa en anpassad [typ av känslig information.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="91514-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="91514-115">**Testa en DLP-princip**</span><span class="sxs-lookup"><span data-stu-id="91514-115">**Test a DLP policy**</span></span>

<span data-ttu-id="91514-116">Om du vill testa dina data med en inbyggd  eller anpassad typ av känslig information använder du alternativet Testtyp under **Klassificeringar**–  >  **känslig information.**</span><span class="sxs-lookup"><span data-stu-id="91514-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="91514-117">Mer information finns i Testa [anpassade typer av känslig information.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="91514-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="91514-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="91514-118">**Reports**</span></span>
  
- <span data-ttu-id="91514-119">Få känsliga datainsikter [med DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="91514-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="91514-120">Visa specifik information om händelsen med en [incidentrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="91514-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
