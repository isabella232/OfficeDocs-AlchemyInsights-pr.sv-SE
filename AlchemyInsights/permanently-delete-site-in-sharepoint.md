---
title: Ta bort en webbplats permanent i SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944329"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Ta bort en webbplats permanent i SharePoint

Om du vill återanvända en URL-adress från en borttagen webbplats (för att återskapa en webbplats) eller om du vill ta bort en webbplats permanent eftersom den inte längre används, kan du använda **Ta bort** permanent från det nya administrationscentret för SharePoint. 

1. Gå till sidan [Borttagna webbplatser i det nya administrationscentret för SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) och logga in med ett konto som har administratörsbehörighet för din organisation. 

2. Välj en webbplats i vänstra kolumnen. 

3. Klicka på **Ta bort permanent**. 

**Obs**! gruppanslutna webbplatser kan inte tas bort permanent från det nya administrationscentret för SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) måste istället användas.  

Se [Ta bort en webbplats permanent](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) för mer information. 
