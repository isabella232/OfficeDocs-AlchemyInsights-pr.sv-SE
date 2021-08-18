---
title: Felkods-0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Om du får ett felmeddelande när du aktiverar Office 2013 för Fjärrskrivbordstjänster (RDS) kan du överväga att aktivera ADAL genom att redigera registret.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316704"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Ett fel uppstod under Office 2013 på Fjärrskrivbordstjänster

Om du får ett felmeddelande när du aktiverar Office 2013 för Fjärrskrivbordstjänster (RDS) kan du överväga att aktivera ADAL genom att redigera registret.
  
|**Registernyckel**|**Typ**|**Värde**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Mer information finns i Aktivera [modern autentisering för Office 2013 på Windows enheter.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Obs!** ADAL är aktiverat som standard i Microsoft 365-appar för företag och Office 2016. Remote Desktop Services (RDS) hette tidigare Terminal Services.
  