---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715902"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomsten i SharePoint eller OneDrive

I SharePoint och OneDrive begränsar du åtkomsten till objekt som filer, mappar och listor genom att endast bevilja åtkomst till grupper eller personer som du vill ha åtkomst till. Som standard ärvs behörigheter i SharePoint från högre upp i hierarkin. Så en fil ärver sina behörigheter från mappen, som ärver dess behörigheter från biblioteket, som ärver dess behörigheter från webbplatsen.
  
Du kan dela på en högre nivå (till exempel genom att dela en hel webbplats) och sedan bryta arv om du inte vill dela alla objekt på webbplatsen. Vi rekommenderar dock inte detta eftersom det gör det mer komplicerat och förvirrande att behålla behörigheterna i framtiden. Här är vad du kan göra istället:
  
- Om du till exempel vill dela allt innehåll i en mapp utom en fil i den flyttar du filen till en ny plats som inte delas.
    
- Om du har två undermappar i en mapp och vill dela en undermapp med grupperna A och B och endast tillåta grupp A-åtkomst till den andra undermappen delar du den överordnade mappen med grupp A och lägger till grupp B i den första undermappen.
    
[Sluta dela en fil eller mapp](https://go.microsoft.com/fwlink/?linkid=2008861)
  

