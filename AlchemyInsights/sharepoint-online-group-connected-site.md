---
title: Lägga till en grupp till en SharePoint-webbplats
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507865"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problem när du skapar eller grupp anslutna webbplatser i SharePoint Online

Det finns några vanliga problem som kan uppstå när Skapa eller återskapa en grupp ansluten plats.

 Om du har tagit bort en grupp och dess anslutna platsen och vill skapa en annan webbplats med samma URL, måste du ta bort den tidigare webbplatsen.

Hämta [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Mer information om att komma igång med powershell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Ta bort webbplatsen från bort platser med hjälp av powershell-cmdlet för [Ta bort SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Om du skapar en grupp ansluten plats och en varning redan finns en annan grupp med samma alias, kontrollera befintliga grupper från [Office 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Kopplad till problemet, ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat alias.

Det finns olika sätt att skapa och använda moderna grupper med SharePoint.

Du kan ansluta befintliga webbplatser till en Office 365-grupp. Mer information finns i [ansluta en Office 365-grupp med hjälp av ineterface för SharePoint-användare](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Om du vill skapa en Office 365-grupp ansluten plats måste du skapa en gruppwebbplats. Mer information finns i [Skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

