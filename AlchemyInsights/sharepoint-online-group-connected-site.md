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
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318142"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Vanliga problem när du skapar en gruppansluten webbplats i SharePoint

1. Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma URL måste du ta bort den tidigare webbplatsen permanent.

   - Ladda [ned SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Mer information om hur du kommer igång med Powershell finns i [Komma igång med SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Ta bort webbplatsen från Borttagna webbplatser med hjälp av [powershell-cmdleten Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell krävs för att permanent ta bort gruppwebbplatser.

1. Om du skapar en gruppansluten webbplats och får en varning: En annan grupp med samma **alias** finns redan kontrollerar du de befintliga grupperna från [Administrationscenter för Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs, eller skapa webbplatsen med ett annat alias tilldelat.

1. Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

   - Du kan ansluta befintliga webbplatser till en Microsoft 365 grupp. Mer information finns i skapa [Anslut Microsoft 365 grupp med hjälp SharePoint användargränssnittet.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Om du vill Microsoft 365 webbplats som är kopplad till en grupp måste du skapa en [gruppwebbplats.](https://admin.microsoft.com/sharepoint)
