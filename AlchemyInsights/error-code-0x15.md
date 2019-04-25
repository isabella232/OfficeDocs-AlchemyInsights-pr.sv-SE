---
title: Felkod 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402757"
---
<span data-ttu-id="0bb23-103">Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret.</span><span class="sxs-lookup"><span data-stu-id="0bb23-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="0bb23-104">**Registernyckel**</span><span class="sxs-lookup"><span data-stu-id="0bb23-104">**Registry key**</span></span>|<span data-ttu-id="0bb23-105">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0bb23-105">**Type**</span></span>|<span data-ttu-id="0bb23-106">**Värde**</span><span class="sxs-lookup"><span data-stu-id="0bb23-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0bb23-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="0bb23-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="0bb23-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="0bb23-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="0bb23-109">1</span><span class="sxs-lookup"><span data-stu-id="0bb23-109">1</span></span>  <br/> |
   
<span data-ttu-id="0bb23-110">Mer information finns i [Aktivera moderna autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="0bb23-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="0bb23-111">ADAL är aktiverat som standard i Office 365 ProPlus och Office 2016.</span><span class="sxs-lookup"><span data-stu-id="0bb23-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="0bb23-112">> remote Desktop Services (RDS) kallades tidigare för Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="0bb23-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

