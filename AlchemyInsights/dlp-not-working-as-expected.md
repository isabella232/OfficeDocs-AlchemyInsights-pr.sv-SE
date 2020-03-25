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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932640"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="6f7b2-102">DLP fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="6f7b2-102">DLP not working as expected</span></span>

<span data-ttu-id="6f7b2-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6f7b2-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6f7b2-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6f7b2-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6f7b2-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6f7b2-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="6f7b2-109">**Konfigurera DLP**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-109">**Setting up DLP**</span></span>

<span data-ttu-id="6f7b2-110">Har du problem med **att DLP (Data Loss Prevention)** i Office 365 inte fungerar som förväntat?</span><span class="sxs-lookup"><span data-stu-id="6f7b2-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="6f7b2-111">Om så är fallet, se till att **DLP-principen** är korrekt konfigurerad och att dina data innehåller vad **DLP-principen** söker när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="6f7b2-112">Med DLP-principer kan du identifiera och skydda känslig information i organisationen.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="6f7b2-113">Om du vill konfigurera DLP-principer använder du informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="6f7b2-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="6f7b2-114">**Vad DLP-principer letar efter**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="6f7b2-115">När du använder de **inbyggda känsliga informationstyperna** i Office 365 Security and Compliance Center söker DLP-principer efter specifika mönster och element när du identifierar dessa känsliga typer.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="6f7b2-116">**Inbyggda typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="6f7b2-117">Information om de inbyggda känsliga typerna och vad en DLP-princip söker efter när du identifierar typen Känslig finns i: [Vilka känsliga informationstyper som söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="6f7b2-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="6f7b2-118">**Anpassade typer av känslig information**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="6f7b2-119">Om du försöker skapa anpassade typer av känslig information använder du följande artikel för information om hur du skapar en anpassad känslig typ: [Skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6f7b2-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="6f7b2-120">**Testa en DLP-princip**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-120">**Test a DLP policy**</span></span>

<span data-ttu-id="6f7b2-121">Om du vill testa dina data med en inbyggd eller anpassad känslig informationstyp använder du alternativet **Testtyp** under Klassificeringar känsliga **informationstyper** > **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="6f7b2-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6f7b2-122">Mer information finns i [Testa anpassade typer av känslig information](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="6f7b2-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="6f7b2-123">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="6f7b2-123">**Reports**</span></span>
  
- <span data-ttu-id="6f7b2-124">Hämta känsliga datainsikter med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="6f7b2-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="6f7b2-125">Se specifik information om händelsen med en [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="6f7b2-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
