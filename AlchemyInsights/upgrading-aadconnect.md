---
title: 932 uppgraderar AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806057"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="d2e02-102">Uppgradera Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d2e02-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="d2e02-103">Automatisk uppgradering är aktive rad som standard för Azure AD Connect, vilket säkerställer att du kör den senaste versionen.</span><span class="sxs-lookup"><span data-stu-id="d2e02-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="d2e02-104">Om du vill kontrol lera inställningarna för automatisk uppgradering använder du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2e02-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="d2e02-105">Cmdleten returnerar ett av följande värden:</span><span class="sxs-lookup"><span data-stu-id="d2e02-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="d2e02-106">**Enabled**: automatisk uppgradering är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="d2e02-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="d2e02-107">**Disabled**: automatisk uppgradering är inaktiverat.</span><span class="sxs-lookup"><span data-stu-id="d2e02-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="d2e02-108">**Upphävda**: systemet är inte längre berättigat att få automatiska uppgraderingar.</span><span class="sxs-lookup"><span data-stu-id="d2e02-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="d2e02-109">Det går inte att konfigurera det här värdet; Det är inställt av systemet.</span><span class="sxs-lookup"><span data-stu-id="d2e02-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="d2e02-110">Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="d2e02-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="d2e02-111">Om du vill ladda ned den senaste versionen av Azure AD Connect går du till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="d2e02-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
