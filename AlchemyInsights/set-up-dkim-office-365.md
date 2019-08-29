---
title: Setup DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666282"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="624c5-102">Setup DKIM i Office 365</span><span class="sxs-lookup"><span data-stu-id="624c5-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="624c5-103">Fullständiga instruktioner för hur du konfigurerar DKIM för anpassade domäner i Office 365 är [här](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="624c5-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="624c5-104">För **varje** egen domän måste du skapa **två** DKIM CNAME-poster i din domän DNS-värdtjänsten (vanligtvis domänregistrerare).</span><span class="sxs-lookup"><span data-stu-id="624c5-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="624c5-105">Till exempel contoso.com och fourthcoffee.com kräver fyra DKIM CNAME-poster: två för contoso.com och två för fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="624c5-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="624c5-106">DKIM CNAME-poster för **varje** anpassad domän använder du följande format:</span><span class="sxs-lookup"><span data-stu-id="624c5-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="624c5-107">**Värdnamn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="624c5-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="624c5-108">**Punkter till adressen eller värde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="624c5-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="624c5-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="624c5-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="624c5-110">**Värdnamn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="624c5-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="624c5-111">**Punkter till adressen eller värde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="624c5-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="624c5-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="624c5-112">**TTL**: 3600</span></span>

   <span data-ttu-id="624c5-113">\<DomainGUID\> står till vänster om `.mail.protection.outlook.com` i anpassade MX-posten för den egna domänen (till exempel `contoso-com` för domänen contoso.com).</span><span class="sxs-lookup"><span data-stu-id="624c5-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="624c5-114">\<InitialDomain\> är den domän som du använde när du registrerade dig för Office 365 (till exempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="624c5-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="624c5-115">När du har skapat CNAME-poster för egna domäner, slutför du följande anvisningar:</span><span class="sxs-lookup"><span data-stu-id="624c5-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="624c5-116">en.</span><span class="sxs-lookup"><span data-stu-id="624c5-116">a.</span></span> <span data-ttu-id="624c5-117">[Logga in på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med ditt arbets- eller skolkonto.</span><span class="sxs-lookup"><span data-stu-id="624c5-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="624c5-118">b.</span><span class="sxs-lookup"><span data-stu-id="624c5-118">b.</span></span> <span data-ttu-id="624c5-119">Välj ikonen för startprogrammet i det övre vänstra hörnet och välj **Admin**.</span><span class="sxs-lookup"><span data-stu-id="624c5-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="624c5-120">c.</span><span class="sxs-lookup"><span data-stu-id="624c5-120">c.</span></span> <span data-ttu-id="624c5-121">Expandera **Admin** och välj **Exchange**i den nedre vänstra navigeringen.</span><span class="sxs-lookup"><span data-stu-id="624c5-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="624c5-122">d.</span><span class="sxs-lookup"><span data-stu-id="624c5-122">d.</span></span> <span data-ttu-id="624c5-123">Gå till **skydd** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="624c5-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="624c5-124">e.</span><span class="sxs-lookup"><span data-stu-id="624c5-124">e.</span></span> <span data-ttu-id="624c5-125">Välj domän och välj **Aktivera** för att **signera meddelanden för den här domänen med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="624c5-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="624c5-126">Upprepa detta steg för varje egen domän.</span><span class="sxs-lookup"><span data-stu-id="624c5-126">Repeat this step for each custom domain.</span></span>
