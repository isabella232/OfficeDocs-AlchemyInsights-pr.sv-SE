---
title: 401 Obehörigt fel i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890284"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Obehörigt fel i SharePoint

Om du får felmeddelandet "(401) Obehörig" i SharePoint kan det vara relaterat till utfasningen av TLS 1.0/1.1. Mer information finns i:

- [Förbereda för TLS 1.2 i Office 365 och Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentiseringsfel inträffar om klienten inte har stöd för TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Uppdatera för att aktivera TLS 1.1 och TLS 1.2 som standard säkra protokoll i WinHTTP i Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Om användarna har TLS-Windows 7 kontrollerar du att de kontrollerar [TLS-chiffersviterna i Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)