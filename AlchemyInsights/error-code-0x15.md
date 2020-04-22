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
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703156"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fel vid aktivering av Office 2013 på fjärrskrivbordstjänster

Om du får ett felmeddelande när du aktiverar Office 2013 på RDS-distributioner (Remote Desktop Services) kan du aktivera ADAL genom att redigera registret.
  
|**Registernyckel**|**Typ**|**Värde**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Programvara\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Mer information finns i [Aktivera modern autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL är aktiverat som standard i Microsoft 365 Apps för företag och Office 2016. Rds (Remote Desktop Services) hette tidigare Terminal Services.
  