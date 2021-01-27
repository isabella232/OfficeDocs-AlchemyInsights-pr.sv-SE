---
title: Ta bort eller återställa program
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015019"
---
# <a name="delete-or-restore-applications"></a>Ta bort eller återställa program

**Så här tar du bort ett program från din Azure AD-klient organisation**:

1. Välj **företags program** i **Azure AD-portalen**. Leta sedan reda på och välj det program du vill ta bort.
2. I avsnittet **Hantera** i det vänstra fönstret väljer du **Egenskaper**.
3. Välj **ta bort** och välj sedan **Ja** för att bekräfta att du vill ta bort appen från din Azure AD-klient.

Mer information om hur du tar bort ett program finns i [snabb start: ta bort ett program från din Azure Active Directory-klient organisation](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

I PowerShell tar [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet bort programproxy-konfigurationer från ett visst program i Azure Active Directory och kan ta bort programmet helt och hållet.

Du kan **återställa ett borttaget program** med PowerShell. När du har identifierat det program du vill återställa kan du återställa det med hjälp av [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
