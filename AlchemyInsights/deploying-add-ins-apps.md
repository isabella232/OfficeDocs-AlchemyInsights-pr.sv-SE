---
title: Distribuera tillägg för Microsoft 365 program
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233552"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Distribuera tillägg för Microsoft 365 program

Centraliserad distribution är det rekommenderade sättet Office distribuera tillägg till användare och grupper inom organisationen. Följ stegen nedan för att distribuera tillägg:

**Obs!** Information om hur du installerar tillägg Office enskilda användare finns i Visa, hantera och installera tillägg [i Office program.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Se också till att enskilda Office Store-tillägg är aktiverat. Mer information finns i Förhindra att tillägg hämtas genom att stänga av Office Store för alla klienter [(utom Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Kontrollera att miljön uppfyller kraven för distribution av tillägg med hjälp av centraliserad distribution. Mer information finns i [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Gå **Inställningar**  >  **appar Skaffa**  >  **appar** i administrationscentret Microsoft 365 och distribuera tillägg. 

Kommentarer: 

- Integrerade appar kräver att administratören har global administratör Exchange administratörsbehörighet.

- När du distribuerar tillägg till flera användare rekommenderar vi att du gör tilldelningar genom att använda grupper istället för enskilda användare. Mer information finns i [Att tänka på när du tilldelar ett tillägg till användare och grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centraliserad distribution stöder inte användare i kapslade grupper eller grupper som har överordnade grupper. Mer information finns i [Användar- och gruppuppgifter.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Kontrollera att Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') har aktiverats för användarna att logga in. Mer information finns i [Konfigurera appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Om du får problem med att distribuera tillägg med hjälp av integrerade appar kan du prova att [distribuera med hjälp av tillägg.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Mer information finns i:

[Distribuera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Hantera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Använda PowerShell-cmdlets för](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) centraliserad distribution för att hantera tillägg 
 [Publicera Office tillägg med hjälp av centraliserad distribution via Microsoft 365 administrationscenter](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Felsökning: Användaren ser inte tillägg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Felsöka användarfel med Office tillägg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)