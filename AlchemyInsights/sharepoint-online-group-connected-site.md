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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051119"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problem när du skapar eller grupperar anslutna platser i SharePoint Online

Det finns ett par vanliga problem som uppstår när du skapar eller återskapar en grupp ansluten webbplats.

 Om du har raderat en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma webbadress måste du ta bort den tidigare webbplatsen permanent.

Hämta [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Mer information om att komma igång med PowerShell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Ta bort webbplatsen från borttagna webbplatser med hjälp av [denTa bort SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdlet.

Om du skapar en grupp ansluten webbplats och får en varning en annan grupp med samma alias redan finns, kontrollera befintliga grupper från [Office 365 från administratörs Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat alias tilldelat.

Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

Du kan ansluta befintliga webbplatser till en Office 365-grupp. Mer information finns [i ansluta en Office 365-grupp med hjälp av SharePoint-användaren ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Om du vill skapa en Office 365-grupp ansluten webbplats måste du skapa en gruppwebbplats. Mer information finns [i skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

