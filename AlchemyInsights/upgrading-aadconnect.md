---
title: 932 uppgradera AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506101"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="8334d-102">Uppgradering av Azure AD Anslut</span><span class="sxs-lookup"><span data-stu-id="8334d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="8334d-103">Som standard aktiveras automatisk uppgradering för Azure AD Connect, som hjälper till att se till att du kör den senaste versionen.</span><span class="sxs-lookup"><span data-stu-id="8334d-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="8334d-104">Om du vill kontrollera inställningarna för automatisk uppgradering använder du cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8334d-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="8334d-105">Cmdlet returnerar ett av följande värden:</span><span class="sxs-lookup"><span data-stu-id="8334d-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="8334d-106">**Aktiverad**: automatisk uppgradering är aktiverad.</span><span class="sxs-lookup"><span data-stu-id="8334d-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="8334d-107">**Inaktiverad**: automatisk uppgradering har inaktiverats.</span><span class="sxs-lookup"><span data-stu-id="8334d-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="8334d-108">**Suspended**: systemet inte längre är berättigad till automatiska uppgraderingar.</span><span class="sxs-lookup"><span data-stu-id="8334d-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="8334d-109">Du kan inte konfigurera den här värde. den anges av systemet.</span><span class="sxs-lookup"><span data-stu-id="8334d-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="8334d-110">Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="8334d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="8334d-111">Om du vill hämta den senaste versionen av Azure AD Connect, gå till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="8334d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
