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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941086"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="2875d-102">DLP fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="2875d-102">DLP not working as expected</span></span>

<span data-ttu-id="2875d-103">Har du problem med **Data förlust Prevention (DLP)** i Office 365 fungerar inte som förväntat?</span><span class="sxs-lookup"><span data-stu-id="2875d-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="2875d-104">Om så är fallet, kontrollera att din **DLP princip** har konfigurerats korrekt och att dina data innehåller vilken **DLP princip** söker efter när det utvärderas.</span><span class="sxs-lookup"><span data-stu-id="2875d-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="2875d-105">**Ställa in DLP**</span><span class="sxs-lookup"><span data-stu-id="2875d-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="2875d-106">DLP-principer kan du identifiera och skydda känslig information i din organisation.</span><span class="sxs-lookup"><span data-stu-id="2875d-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="2875d-107">Inställningar för DLP-principer genom att använda informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="2875d-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="2875d-108">**DLP-principer leta efter**</span><span class="sxs-lookup"><span data-stu-id="2875d-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="2875d-109">När du använder **inbyggda känslig informationstyper** i Office 365 säkerhet och överensstämmelse center leta DLP principer efter särskilda mönster och element när upptäcka sådana känsliga.</span><span class="sxs-lookup"><span data-stu-id="2875d-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="2875d-110">**Typer av inbyggda känslig Information**</span><span class="sxs-lookup"><span data-stu-id="2875d-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="2875d-111">Information om de inbyggda känsliga typerna och en DLP-princip ser för när identifiera känsliga typen finns: [letar du vilka av känslig information](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2875d-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2875d-112">**Typer av anpassade känslig Information**</span><span class="sxs-lookup"><span data-stu-id="2875d-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="2875d-113">Om du vill skapa anpassade känslig information, Använd följande artikel för information om hur du skapar en anpassad känsliga typ: [Skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2875d-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="2875d-114">**Testa en DLP-princip**</span><span class="sxs-lookup"><span data-stu-id="2875d-114">**Test a DLP policy**</span></span>

<span data-ttu-id="2875d-115">Om du vill testa dina data med en inbyggd eller anpassad känslig information använder du alternativet **Testa typ** under **klassificeringar** > **informationstyper av känslig**.</span><span class="sxs-lookup"><span data-stu-id="2875d-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="2875d-116">Mer information finns i [anpassade känslig information testtyper](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="2875d-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="2875d-117">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="2875d-117">**Reports**</span></span>
  
- <span data-ttu-id="2875d-118">Hämta känsliga data insikter med [DLP rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="2875d-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="2875d-119">Se specifika detaljer om händelsen med en [Rapport om incidenten](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="2875d-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
