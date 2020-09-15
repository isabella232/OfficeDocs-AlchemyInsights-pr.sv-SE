---
title: Felkod 0x15
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
description: Om du får ett fel meddelande när du aktiverar Office 2013 på klient distributioner för fjärr skrivbord kan du överväga att aktivera ADAL genom att redigera registret.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709205"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fel vid aktivering av Office 2013 på fjärr skrivbords tjänster

Om du får ett fel meddelande när du aktiverar Office 2013 på klient distributioner för fjärr skrivbord kan du överväga att aktivera ADAL genom att redigera registret.
  
|**Registernyckel**|**Typ**|**Värde**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |9.1  <br/> |

Mer information finns i [Aktivera modern auktorisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL är aktiverat som standard i Microsoft 365-appar för Enterprise och Office 2016. Fjärr skrivbords tjänster (RDS) hette tidigare Terminal Services.
  