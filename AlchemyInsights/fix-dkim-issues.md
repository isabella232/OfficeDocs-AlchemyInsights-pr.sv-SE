---
title: Åtgärda problem vid installation av DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765461"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="2c311-102">Åtgärda problem vid installation av DKIM</span><span class="sxs-lookup"><span data-stu-id="2c311-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="2c311-103">Om du har problem att aktivera DKIM för din egen domän, gör du följande:</span><span class="sxs-lookup"><span data-stu-id="2c311-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="2c311-104">De flesta problem vid installation av DKIM är relaterade till felaktiga DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="2c311-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="2c311-105">Kontrollera DKIM CNAME-posten (**inte** en TXT-post) är korrekt formaterad.</span><span class="sxs-lookup"><span data-stu-id="2c311-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="2c311-106">Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2c311-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="2c311-107">När du skapar eller uppdatera DKIM DNS-poster i DNS-värdtjänsten för din domän (vanligtvis din domänregistrerare), vänta på att sprida DNS-posterna.</span><span class="sxs-lookup"><span data-stu-id="2c311-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="2c311-108">Om du inte kan skapa DKIM DNS-poster i administratörscenter, kan du ersätta \<CustomDomain\> med din egen domän (till exempel contoso.com) och kör detta kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="2c311-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
