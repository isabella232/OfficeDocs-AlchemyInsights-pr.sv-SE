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
Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret. 
  
|**Registernyckel**|**Typ**|**Värde**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Mer information finns i [Aktivera moderna autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL är aktiverat som standard i Office 365 ProPlus och Office 2016. > remote Desktop Services (RDS) kallades tidigare för Terminal Services. 
  

