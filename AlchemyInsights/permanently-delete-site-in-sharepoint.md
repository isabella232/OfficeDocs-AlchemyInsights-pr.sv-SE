---
title: Ta bort en webbplats permanent i SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955235"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Ta bort en webbplats permanent i SharePoint

Om du vill återanvända en URL-adress från en borttagen webbplats (för att återskapa en webbplats) eller om du vill ta bort en webbplats permanent eftersom den inte längre används, kan du använda **Ta bort** permanent från det nya administrationscentret för SharePoint. 

1. Gå till sidan [Borttagna webbplatser i det nya administrationscentret för SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) och logga in med ett konto som har administratörsbehörighet för din organisation. 

2. Välj en webbplats i vänstra kolumnen. 

3. Klicka på **Ta bort permanent**. 

**Obs**! gruppanslutna webbplatser kan inte tas bort permanent från det nya administrationscentret för SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) måste istället användas.  

Se [Ta bort en webbplats permanent](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) för mer information. 
