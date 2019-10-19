---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551469"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomsten i SharePoint eller OneDrive

I SharePoint och OneDrive begränsar du åtkomsten till objekt som filer, mappar och listor genom att endast bevilja åtkomst till grupper eller personer som du vill ha åtkomst till. Som standard ärvs behörigheterna i SharePoint från högre upp i hierarkin. Så en fil ärver sina behörigheter från mappen, som ärver sina behörigheter från biblioteket, som ärver dess behörigheter från platsen.
  
Du kan dela på en högre nivå (till exempel genom att dela en hel webbplats) och sedan bryta arv om du inte vill dela alla objekt på webbplatsen. Men vi rekommenderar inte detta eftersom det gör att underhålla behörigheterna mer komplexa och förvirrande i framtiden. Det här kan du göra i stället:
  
- Om du till exempel vill dela allt innehåll i en mapp med undantag för en fil i den, flyttar du filen till en ny plats som inte delas.
    
- Om du har två undermappar i en mapp och du vill dela en undermapp med grupperna A och B och endast tillåta grupp A-åtkomst till den andra undermappen, delar du den överordnade mappen med grupp A och lägger till grupp B i den första undermappen.
    
[Sluta dela en fil eller mapp](https://go.microsoft.com/fwlink/?linkid=2008861)
  

