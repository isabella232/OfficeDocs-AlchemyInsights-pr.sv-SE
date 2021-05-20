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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539950"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="5caf7-102">401 Obehörigt fel i SharePoint</span><span class="sxs-lookup"><span data-stu-id="5caf7-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="5caf7-103">Om du får felmeddelandet "(401) Obehörig" i SharePoint kan det vara relaterat till utfasningen av TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="5caf7-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="5caf7-104">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="5caf7-104">For more info, see:</span></span>

- [<span data-ttu-id="5caf7-105">Förbereda för TLS 1.2 i Office 365 och Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="5caf7-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="5caf7-106">Autentiseringsfel inträffar om klienten inte har stöd för TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="5caf7-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="5caf7-107">Uppdatera för att aktivera TLS 1.1 och TLS 1.2 som standard säkra protokoll i WinHTTP i Windows</span><span class="sxs-lookup"><span data-stu-id="5caf7-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="5caf7-108">Om användarna har Windows 7 kontrollerar du att de kontrollerar [TLS-chiffersviterna i Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="5caf7-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>