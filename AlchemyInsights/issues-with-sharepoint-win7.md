---
title: Problem med SharePoint på Windows 7-datorer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125519"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="76762-102">Problem med SharePoint på Windows 7-datorer</span><span class="sxs-lookup"><span data-stu-id="76762-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="76762-103">Om du får felmeddelanden på Windows 7-datorer när du arbetar med SharePoint eller OneDrive kan de vara relaterade till utfasningen av TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="76762-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="76762-104">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="76762-104">For more information, see:</span></span>

- [<span data-ttu-id="76762-105">Förbereda för TLS 1.2 i Office 365 och Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="76762-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="76762-106">Windows 7 SP1/Windows 8 klienter måste ha TLS1.2 aktiverat.</span><span class="sxs-lookup"><span data-stu-id="76762-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="76762-107">Mer information finns i [Autentiseringsfel uppstår när klienten inte har stöd för TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="76762-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="76762-108">Installera KB3140245 och skapa registervärdet.</span><span class="sxs-lookup"><span data-stu-id="76762-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="76762-109">Mer information finns i Uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) som standard säkra protokoll i WinHTTP i Windows</span><span class="sxs-lookup"><span data-stu-id="76762-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="76762-110">Windows 7 SP1/Windows 8 måste säkerställa att de senaste TLS-chiffersviterna installeras.</span><span class="sxs-lookup"><span data-stu-id="76762-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="76762-111">Mer information finns i [Microsoft Security Advisory 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)</span><span class="sxs-lookup"><span data-stu-id="76762-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


