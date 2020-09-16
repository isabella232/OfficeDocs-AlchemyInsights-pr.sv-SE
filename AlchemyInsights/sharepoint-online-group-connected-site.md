---
title: Lägga till en grupp på en SharePoint-webbplats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771226"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problem med att skapa en gruppansluten webbplats i SharePoint

1. Några vanliga problem inträffade när du skapade eller återskapade en grupp webbplats.
Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en ny webbplats med samma URL måste du ta bort den föregående webbplatsen permanent.

   - Ladda ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Mer information om hur du kommer igång med PowerShell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Ta bort webbplatsen från borttagna webbplatser med PowerShell-cmdleten [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell krävs för att permanent ta bort grupp webbplatser.

1. Om du skapar en sammankopplad webbplats och får ett varnings meddelande: **en annan grupp med samma alias finns**i [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat tilldelat alias.

1. Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

   - Du kan ansluta befintliga webbplatser till en Microsoft 365-grupp. Mer information finns i [ansluta en Microsoft 365-grupp med användar gränssnittet i SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Om du vill skapa en Microsoft 365-gruppansluten webbplats måste du skapa en [grupp webbplats](https://admin.microsoft.com/sharepoint).
