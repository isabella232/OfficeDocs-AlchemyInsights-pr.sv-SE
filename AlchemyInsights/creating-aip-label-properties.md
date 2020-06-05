---
title: Skapa AIP-etikettprinciper
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569513"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="73d18-102">Skapa AIP-etikettprinciper</span><span class="sxs-lookup"><span data-stu-id="73d18-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="73d18-103">Azure Information Protection(AIP) etiketter kan användas med hela skalan av data som en organisation vanligtvis skapar och lagrar, från den lägsta klassificeringen av personuppgifter, till den högsta klassificeringen av mycket konfidentiella data.</span><span class="sxs-lookup"><span data-stu-id="73d18-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="73d18-104">Azure Information Protection Policies gäller för den klassiska Azure Information Protection(AIP) klassiska klienten och inte [AIP Unified Labeling-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="73d18-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="73d18-105">Du kan konfigurera flera element i en AIP-princip, inklusive alternativ som:</span><span class="sxs-lookup"><span data-stu-id="73d18-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="73d18-106">Alternativ för vilken etikett låter administratörer eller användare klassificera och skydda (valfria) dokument och e-postmeddelanden</span><span class="sxs-lookup"><span data-stu-id="73d18-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="73d18-107">Möjlighet att tillämpa klassificering när användare sparar dokument och skickar e-post</span><span class="sxs-lookup"><span data-stu-id="73d18-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="73d18-108">Möjlighet att automatiskt märka ett e-postmeddelande, baserat på dess bilagor.</span><span class="sxs-lookup"><span data-stu-id="73d18-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="73d18-109">Alternativ för att styra om informationsskyddsfältet visas i Office-program</span><span class="sxs-lookup"><span data-stu-id="73d18-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="73d18-110">Fler alternativ och information om Azure Information Protection-principer finns i Översikt [över Azure-informationsskyddsprincipen](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="73d18-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="73d18-111">Andra användbara resurser när det gäller AIP-principer finns i:</span><span class="sxs-lookup"><span data-stu-id="73d18-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="73d18-112">Självstudiekurs: Konfigurera principinställningar för Azure-informationsskydd och skapa en ny etikett</span><span class="sxs-lookup"><span data-stu-id="73d18-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73d18-113">Konfigurera principen för skydd av Azure-information</span><span class="sxs-lookup"><span data-stu-id="73d18-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="73d18-114">Skapa och konfigurera känslighetsetiketter och deras principer</span><span class="sxs-lookup"><span data-stu-id="73d18-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="73d18-115">Hjälpguider för vanliga scenarier som använder Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="73d18-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="73d18-116">Granska Azure Information Protection-dokumentation</span><span class="sxs-lookup"><span data-stu-id="73d18-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="73d18-117">Krav för Azure-informationsskydd</span><span class="sxs-lookup"><span data-stu-id="73d18-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="73d18-118">Snabbstartshandledning för Azure-informationsskydd</span><span class="sxs-lookup"><span data-stu-id="73d18-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="73d18-119">Ladda ned Azure Information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="73d18-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)