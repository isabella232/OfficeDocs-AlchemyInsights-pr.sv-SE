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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problem med SharePoint på Windows 7-datorer

Om du får felmeddelanden på Windows 7-datorer när du arbetar med SharePoint eller OneDrive kan de vara relaterade till utfasningen av TLS 1.0/1.1. Mer information finns i:

- [Förbereda för TLS 1.2 i Office 365 och Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 klienter måste ha TLS1.2 aktiverat. Mer information finns i [Autentiseringsfel uppstår när klienten inte har stöd för TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installera KB3140245 och skapa registervärdet. Mer information finns i Uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) som standard säkra protokoll i WinHTTP i Windows

- Windows 7 SP1/Windows 8 måste säkerställa att de senaste TLS-chiffersviterna installeras. Mer information finns i [Microsoft Security Advisory 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


