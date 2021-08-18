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
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317714"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Felet "Den underliggande anslutningen stängdes" i SharePoint

Om du får felet "Den underliggande anslutningen stängdes" i SharePoint kan det vara relaterat till utfasningen av TLS 1.0/1.1. Mer information finns i följande artiklar:

- [Förbereda för TLS 1.2 i Office 365 och Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentiseringsfel inträffar om klienten inte har stöd för TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Uppdatera för att aktivera TLS 1.1 och TLS 1.2 som standard säkra protokoll i WinHTTP i Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Om användarna har Windows 7 kontrollerar du att de kontrollerar [TLS-chiffersviterna i Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)