---
title: 932 Uppgradering av AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766511"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="fd9dc-102">Uppgradera Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="fd9dc-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="fd9dc-103">Som standard är automatisk uppgradering aktiverad för Azure AD Connect, vilket hjälper till att säkerställa att du kör den senaste versionen.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="fd9dc-104">Om du vill verifiera de automatiska uppgraderingsinställningarna använder du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="fd9dc-105">Cmdleten returnerar ett av följande värden:</span><span class="sxs-lookup"><span data-stu-id="fd9dc-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="fd9dc-106">**Aktiverad**: Automatisk uppgradering är aktiverad.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="fd9dc-107">**Inaktiverad**: Automatisk uppgradering är inaktiverad.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="fd9dc-108">**Pausad**: Systemet är inte längre berättigat till automatiska uppgraderingar.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="fd9dc-109">Du kan inte konfigurera det här värdet. den är inställd av systemet.</span><span class="sxs-lookup"><span data-stu-id="fd9dc-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="fd9dc-110">Mer information finns i [Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="fd9dc-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="fd9dc-111">Om du vill hämta den senaste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)versionen av Azure AD Connect går du till .</span><span class="sxs-lookup"><span data-stu-id="fd9dc-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
