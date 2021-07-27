---
title: Lägga till en grupp på SharePoint webbplats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532237"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Vanliga problem när du skapar en gruppansluten webbplats i SharePoint

1. Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma URL måste du ta bort den tidigare webbplatsen permanent.

   - Ladda [ned SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Mer information om hur du kommer igång med Powershell finns i [Komma igång med SharePoint Online Management Shell.](/powershell/module/sharepoint-online/remove-sposite)
   - Ta bort webbplatsen från Borttagna webbplatser med hjälp av [powershell-cmdleten Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell krävs för att permanent ta bort gruppwebbplatser.

1. Om du skapar en gruppansluten webbplats och får en varning: En annan grupp med samma **alias** finns redan kontrollerar du de befintliga grupperna från [Administrationscenter för Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs, eller skapa webbplatsen med ett annat alias tilldelat.

1. Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

   - Du kan ansluta befintliga webbplatser till en Microsoft 365 grupp. Mer information finns i Anslut [en Microsoft 365-grupp med SharePoint användargränssnittet.](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Om du vill Microsoft 365 webbplats som är kopplad till en grupp måste du skapa en [gruppwebbplats.](https://admin.microsoft.com/sharepoint)
