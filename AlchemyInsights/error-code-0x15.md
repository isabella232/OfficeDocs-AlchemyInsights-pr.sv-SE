---
title: Felkod 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Om du får ett felmeddelande när du aktiverar Office 2013 på RDS-distributioner (Remote Desktop Services) kan du aktivera ADAL genom att redigera registret.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506864"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="d769f-103">Fel vid aktivering av Office 2013 på fjärrskrivbordstjänster</span><span class="sxs-lookup"><span data-stu-id="d769f-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="d769f-104">Om du får ett felmeddelande när du aktiverar Office 2013 på RDS-distributioner (Remote Desktop Services) kan du aktivera ADAL genom att redigera registret.</span><span class="sxs-lookup"><span data-stu-id="d769f-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="d769f-105">**Registernyckel**</span><span class="sxs-lookup"><span data-stu-id="d769f-105">**Registry key**</span></span>|<span data-ttu-id="d769f-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="d769f-106">**Type**</span></span>|<span data-ttu-id="d769f-107">**Värde**</span><span class="sxs-lookup"><span data-stu-id="d769f-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d769f-108">HKEY_CURRENT_USER\Programvara\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="d769f-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d769f-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d769f-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d769f-110">1</span><span class="sxs-lookup"><span data-stu-id="d769f-110">1</span></span>  <br/> |

<span data-ttu-id="d769f-111">Mer information finns i [Aktivera modern autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d769f-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d769f-112">ADAL är aktiverat som standard i Microsoft 365 Apps för företag och Office 2016.</span><span class="sxs-lookup"><span data-stu-id="d769f-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="d769f-113">Rds (Remote Desktop Services) hette tidigare Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="d769f-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  