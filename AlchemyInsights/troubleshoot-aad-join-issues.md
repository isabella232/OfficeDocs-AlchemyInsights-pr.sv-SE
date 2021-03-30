---
title: Felsöka problem med Azure AD-anslutning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405762"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Felsöka problem med Azure AD-anslutning

1. Om du inställningar enhetsregistreringar för första gången bör du kontrollera att du har granskat Introduktion till enhetshantering i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) som vägleder dig om hur du får enheter under kontroll till Azure AD. 
1. Om du registrerar enheter i Azure AD direkt och registrerar dem i Intune måste du se till [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) att du har konfigurerat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) och har licensieringen först.
1. Se till att du har behörighet att utföra åtgärder i Azure AD. Endast en global administratör i Azure AD kan hantera inställningar för enhetsregistreringar.
1. Om du vill implementering av Azure AD-koppling kan du [gå med i Planera Azure AD-anslutning.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Mer information om hur du löser vanliga problem med Azure AD-koppling finns i Vanliga frågor och svar om [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) Join och för Windows 10 Pro-enheter finns i Det går inte att ansluta [Windows 10 Pro-datorn](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) till Azure AD - Behöver uppgradera till - Microsoft Community
