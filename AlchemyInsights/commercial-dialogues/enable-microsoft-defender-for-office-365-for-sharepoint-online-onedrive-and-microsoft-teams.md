---
title: Aktivera Valv bifogade filer för SharePoint Online, OneDrive och Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332397"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera Valv bifogade filer för SharePoint Online, OneDrive och Microsoft Teams

1. Med dina autentiseringsuppgifter som global administratör eller säkerhetsadministratör öppnar du Microsoft 365 Defender-portalen på och går sedan till Principer & regler Hotprinciper <https://security.microsoft.com> **Valv** \>  \> **Bilagor**  i avsnittet Principer

   Om du vill gå direkt **Valv bifogade** filer använder du <https://security.microsoft.com/safeattachmentv2> .

2. På sidan **Valv klickar** du på **Globala inställningar.**
3. På den utfäll du vill visa väljer du Aktivera Microsoft Defender för **Office 365 för SharePoint, OneDrive** och Microsoft Teams och sedan **Spara**.

    **Tips:** Gör följande för att förbättra skyddet för Valv och SharePoint, OneDrive och Microsoft Teams:
    - Om du vill hindra användare från att hämta skadliga filer använder du värdet för `$true` parametern *DisallowInfectedFileDownload* i cmdleten **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** i SharePoint Online PowerShell. Mer information finns i [Använda SharePoint Online PowerShell för att hindra användare från att hämta skadliga filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Skapa en aviseringsprincip för identifierade filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Mer information finns i [Bifoga Valv för Office 365 för SharePoint, OneDrive och Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
