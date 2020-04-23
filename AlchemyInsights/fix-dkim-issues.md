---
title: Åtgärda problem med installation av DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717580"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="838fd-102">Åtgärda problem med installation av DKIM</span><span class="sxs-lookup"><span data-stu-id="838fd-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="838fd-103">Om du får problem med att aktivera DKIM för din anpassade domän gör du så här:</span><span class="sxs-lookup"><span data-stu-id="838fd-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="838fd-104">De flesta DKIM-inställningsproblem är relaterade till felaktiga DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="838fd-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="838fd-105">Kontrollera att DKIM CNAME-posten **(inte** en TXT-post) är korrekt formaterad.</span><span class="sxs-lookup"><span data-stu-id="838fd-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="838fd-106">Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="838fd-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="838fd-107">När du har skapat eller uppdaterat dina DKIM DNS-poster på DNS-värdtjänsten för din domän (vanligtvis domänregistratorer) väntar du på att DNS-posterna ska spridas.</span><span class="sxs-lookup"><span data-stu-id="838fd-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="838fd-108">Om du inte kan skapa DKIM DNS-posterna i \<administrationscentret\> kan du ersätta CustomDomain med din anpassade domän (till `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`exempel contoso.com) och köra det här kommandot i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .</span><span class="sxs-lookup"><span data-stu-id="838fd-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
