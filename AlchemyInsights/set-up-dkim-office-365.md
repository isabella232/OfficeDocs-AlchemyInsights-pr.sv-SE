---
title: Konfigurera DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645690"
---
# <a name="setup-dkim"></a><span data-ttu-id="8cac8-102">Konfigurera DKIM</span><span class="sxs-lookup"><span data-stu-id="8cac8-102">Setup DKIM</span></span>

<span data-ttu-id="8cac8-103">De fullständiga instruktionerna för att konfigurera DKIM för anpassade domäner i Microsoft 365 finns [här](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="8cac8-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="8cac8-104">För **varje** anpassad domän måste du skapa **två** DKIM CNAME-poster på domänens DNS-värdtjänst (vanligtvis domänregistratorer).</span><span class="sxs-lookup"><span data-stu-id="8cac8-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="8cac8-105">Till exempel kräver contoso.com och fourthcoffee.com fyra DKIM CNAME-poster: två för contoso.com och två för fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="8cac8-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="8cac8-106">DKIM CNAME-posterna för **varje** anpassad domän använder följande format:</span><span class="sxs-lookup"><span data-stu-id="8cac8-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="8cac8-107">**Värdnamn:**`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="8cac8-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="8cac8-108">**Pekar på adress eller värde:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="8cac8-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="8cac8-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="8cac8-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="8cac8-110">**Värdnamn:**`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="8cac8-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="8cac8-111">**Pekar på adress eller värde:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="8cac8-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="8cac8-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="8cac8-112">**TTL**: 3600</span></span>

   <span data-ttu-id="8cac8-113">\<DomainGUID\> är texten till `.mail.protection.outlook.com` vänster om i den anpassade MX-posten `contoso-com` för den anpassade domänen (till exempel för domänen contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8cac8-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="8cac8-114">\<InitialDomain\> är den domän som du använde när du registrerade dig för Microsoft 365 (till exempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="8cac8-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="8cac8-115">När du har skapat CNAME-posterna för dina anpassade domäner gör du följande instruktioner:</span><span class="sxs-lookup"><span data-stu-id="8cac8-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="8cac8-116">a.</span><span class="sxs-lookup"><span data-stu-id="8cac8-116">a.</span></span> <span data-ttu-id="8cac8-117">[logga in på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med ditt arbets- eller skolkonto.</span><span class="sxs-lookup"><span data-stu-id="8cac8-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="8cac8-118">b.</span><span class="sxs-lookup"><span data-stu-id="8cac8-118">b.</span></span> <span data-ttu-id="8cac8-119">Välj ikonen för startprogrammet i det övre vänstra hörnet, och välj sedan **Admin**.</span><span class="sxs-lookup"><span data-stu-id="8cac8-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="8cac8-120">C.</span><span class="sxs-lookup"><span data-stu-id="8cac8-120">c.</span></span> <span data-ttu-id="8cac8-121">I den nedre vänstra navigeringen expanderar du **Administratör** och väljer **SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="8cac8-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="8cac8-122">D.</span><span class="sxs-lookup"><span data-stu-id="8cac8-122">d.</span></span> <span data-ttu-id="8cac8-123">Gå till **Skydd** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="8cac8-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="8cac8-124">ᵉ.</span><span class="sxs-lookup"><span data-stu-id="8cac8-124">e.</span></span> <span data-ttu-id="8cac8-125">Välj domänen och välj sedan **Aktivera** för **signeringsmeddelanden för den här domänen med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="8cac8-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="8cac8-126">Upprepa det här steget för varje anpassad domän.</span><span class="sxs-lookup"><span data-stu-id="8cac8-126">Repeat this step for each custom domain.</span></span>
