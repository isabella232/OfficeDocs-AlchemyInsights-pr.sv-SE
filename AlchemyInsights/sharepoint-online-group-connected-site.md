---
title: Lägga till en grupp på en SharePoint-webbplats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064411"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problem när du skapar en gruppansluten webbplats i SharePoint

1. Några vanliga problem uppstod när du skapar eller återskapar en gruppansluten plats.
Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma WEBBADRESS måste du ta bort den tidigare webbplatsen permanent.

   - Ladda ner [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Mer information om hur du kommer igång med Powershell finns i [Komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Ta bort webbplatsen från borttagna platser med hjälp av [cmdleten Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell krävs för att permanent ta bort gruppwebbplatser.

1. Om du skapar en gruppansluten webbplats och får en varning: Det finns redan en **annan grupp med samma alias**kontrollerar du de befintliga grupperna från Administrationscentret för Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups). Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa platsen med ett annat alias tilldelat.

1. Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

   - Du kan ansluta befintliga webbplatser till en Microsoft 365-grupp. Mer information finns i [Ansluta en Microsoft 365-grupp med SharePoint-användargränssnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Om du vill skapa en ansluten microsoft 365-gruppwebbplats måste du skapa en [gruppwebbplats](https://admin.microsoft.com/sharepoint).
