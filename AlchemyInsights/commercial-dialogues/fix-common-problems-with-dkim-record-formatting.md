---
title: Åtgärda vanliga problem med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750755"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="d76fd-102">Åtgärda vanliga problem med DKIM-postformatering</span><span class="sxs-lookup"><span data-stu-id="d76fd-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="d76fd-103">De flesta DKIM-konfigurationsproblem är relaterade till felaktiga DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="d76fd-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="d76fd-104">Om du vill åtgärda dkim-set-up-problemen kontrollerar du att DKIM CNAME-posten **(inte** en TXT-post) är rätt formaterad.</span><span class="sxs-lookup"><span data-stu-id="d76fd-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d76fd-105">Mer information finns i Vad [du behöver göra för att konfigurera DKIM manuellt i Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="d76fd-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="d76fd-106">Om du behöver hjälp med DNS-poster i allmänhet kan du gå till [Skapa DNS-poster på vilken DNS-värd som helst för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="d76fd-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="d76fd-107">När du har skapat eller uppdaterat DKIM DNS-posterna hos DNS-värdtjänsten för din domän måste du vänta på att DNS-posterna har spridits.</span><span class="sxs-lookup"><span data-stu-id="d76fd-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>