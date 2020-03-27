---
title: DLP fungerar inte som förväntat
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977456"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ae474-102">DLP fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="ae474-102">DLP not working as expected</span></span>

<span data-ttu-id="ae474-103">**Viktigt:** Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga – Besök [Tillfälliga funktionsjusteringar](https://aka.ms/ODSPAdjustments) för SharePoint Online för mer information.</span><span class="sxs-lookup"><span data-stu-id="ae474-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="ae474-104">**Konfigurera DLP**</span><span class="sxs-lookup"><span data-stu-id="ae474-104">**Setting up DLP**</span></span>

<span data-ttu-id="ae474-105">Har du problem med **att DLP (Data Loss Prevention)** i Office 365 inte fungerar som förväntat?</span><span class="sxs-lookup"><span data-stu-id="ae474-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ae474-106">Om så är fallet, se till att **DLP-principen** är korrekt konfigurerad och att dina data innehåller vad **DLP-principen** söker när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="ae474-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="ae474-107">Med DLP-principer kan du identifiera och skydda känslig information i organisationen.</span><span class="sxs-lookup"><span data-stu-id="ae474-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="ae474-108">Om du vill konfigurera DLP-principer använder du informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="ae474-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="ae474-109">**Vad DLP-principer letar efter**</span><span class="sxs-lookup"><span data-stu-id="ae474-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ae474-110">När du använder de **inbyggda känsliga informationstyperna** i Office 365 Security and Compliance Center söker DLP-principer efter specifika mönster och element när du identifierar dessa känsliga typer.</span><span class="sxs-lookup"><span data-stu-id="ae474-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ae474-111">**Inbyggda typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="ae474-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ae474-112">Information om de inbyggda känsliga typerna och vad en DLP-princip söker efter när du identifierar typen Känslig finns i: [Vilka känsliga informationstyper som söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="ae474-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ae474-113">**Anpassade typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="ae474-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ae474-114">Om du försöker skapa anpassade typer av känslig information använder du följande artikel för information om hur du skapar en anpassad känslig typ: [Skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ae474-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ae474-115">**Testa en DLP-princip**</span><span class="sxs-lookup"><span data-stu-id="ae474-115">**Test a DLP policy**</span></span>

<span data-ttu-id="ae474-116">Om du vill testa dina data med en inbyggd eller anpassad känslig informationstyp använder du alternativet **Testtyp** under Klassificeringar känsliga **informationstyper** > **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="ae474-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ae474-117">Mer information finns i [Testa anpassade typer av känslig information](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="ae474-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ae474-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="ae474-118">**Reports**</span></span>
  
- <span data-ttu-id="ae474-119">Hämta känsliga datainsikter med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="ae474-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ae474-120">Se specifik information om händelsen med en [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="ae474-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
