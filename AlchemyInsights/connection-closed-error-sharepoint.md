---
title: Det underliggande anslutningsfelet stängdes i SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233444"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Felet "Den underliggande anslutningen stängdes" i SharePoint

Om du får felet "Den underliggande anslutningen stängdes" i SharePoint kan det vara relaterat till utfasningen av TLS 1.0/1.1. Mer information finns i följande artiklar:

- [Förbereda för TLS 1.2 i Office 365 och Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Autentiseringsfel inträffar om klienten inte har stöd för TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Om användarna har Windows 7 kontrollerar du att de kontrollerar [TLS-chiffersviterna i Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)