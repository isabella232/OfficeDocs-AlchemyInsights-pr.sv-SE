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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388263"
---
Om du får ett fel när aktivera Office 2013 på distributioner av Remote Desktop Services (RDS), kan du överväga att aktivera ADAL genom att redigera registret.
  
|**Registernyckel**|**Typ**|**Värde**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Mer information finns i [Aktivera moderna autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL är aktiverat som standard i Office 365 ProPlus och Office 2016. > remote Desktop Services (RDS) kallades tidigare för Terminal Services.
  