---
title: Felkod 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527077"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="c1df0-103">Ett fel uppstod vid aktiveringen av Office 2013 på Remote Desktop Services</span><span class="sxs-lookup"><span data-stu-id="c1df0-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="c1df0-104">Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret.</span><span class="sxs-lookup"><span data-stu-id="c1df0-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="c1df0-105">**Registernyckel**</span><span class="sxs-lookup"><span data-stu-id="c1df0-105">**Registry key**</span></span>|<span data-ttu-id="c1df0-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="c1df0-106">**Type**</span></span>|<span data-ttu-id="c1df0-107">**Värde**</span><span class="sxs-lookup"><span data-stu-id="c1df0-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c1df0-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c1df0-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c1df0-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c1df0-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c1df0-110">1</span><span class="sxs-lookup"><span data-stu-id="c1df0-110">1</span></span>  <br/> |

<span data-ttu-id="c1df0-111">Mer information finns i [Aktivera moderna autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c1df0-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c1df0-112">ADAL är aktiverat som standard i Office 365 ProPlus och Office 2016.</span><span class="sxs-lookup"><span data-stu-id="c1df0-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="c1df0-113">Remote Desktop Services (RDS) kallades tidigare för Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="c1df0-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  