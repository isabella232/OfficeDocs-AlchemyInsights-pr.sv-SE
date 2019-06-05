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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719499"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Skapa grupp ansluten plats i SharePoint Online

<p><strong>Det finns några vanliga problem som kan uppstå när Skapa eller återskapa en grupp ansluten plats.&nbsp;</strong></p>  <p>1.Om du har tagit bort en grupp och dess anslutna platsen och vill skapa en annan webbplats med samma URL, måste du ta bort den tidigare webbplatsen.</p>  <ul>  <li>Hämta <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - för mer information om att komma igång med powershell finns i <a title="komma igång med SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Komma igång med SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Ta bort platsen från bort webbplatser med hjälp av den <a title="ta bort SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Ta bort SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Om du skapar en grupp ansluten plats och få en varning om <strong>en annan grupp med samma alias redan finns</strong>, kontrollera befintliga grupper från den <a title="Office 365 Admin Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 Admin Center</a>. Kopplad till problemet, ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat alias.&nbsp;</p>  <p><strong>Det finns olika sätt att skapa och använda moderna grupper med SharePoint.&nbsp;</strong></p>  <ol>  <li>Du kan ansluta befintliga webbplatser till en Office 365-grupp. Mer information finns i <a title="ansluter en Office 365-grupp med hjälp av ineterface för SharePoint-användare" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Ansluta en Office 365-grupp med hjälp av SharePoint användaren ineterface</a>.</li>  <li>Om du vill skapa en Office 365-grupp ansluten plats måste du skapa en gruppwebbplats. Mer information finns i <a title="skapar en gruppwebbplats i SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Skapa en gruppwebbplats i SharePoint.</a></li>  </ol>

