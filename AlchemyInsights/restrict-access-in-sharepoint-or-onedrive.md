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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551469"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomsten i SharePoint eller OneDrive

I SharePoint och OneDrive kan begränsa du åtkomsten till objekt som filer, mappar och listor genom att bevilja åtkomst till grupper eller användare som du vill ska ha åtkomst. Som standard ärvs behörigheterna i SharePoint från högre upp i hierarkin. Så ärver en fil dess behörigheter från mappen som har ärvt sina rättigheter från biblioteket som ärver dess behörighet från webbplatsen.
  
Du kan dela på en högre nivå (t ex genom att dela en hel webbplats) och sedan bryta arvet om du inte vill dela alla objekt på webbplatsen. Men rekommenderar vi inte detta eftersom det gör att underhålla behörigheter mer komplexa och förvirrande i framtiden. Det här är vad du kan göra i stället:
  
- Om du till exempel vill dela hela innehållet i en mapp med undantag för en fil i den, kan du flytta filen till en ny plats som inte är delad.
    
- Om du har två undermappar i en mapp och du vill dela en undermapp med grupperna A och B och tillåter endast grupp A åtkomsten till undermappen andra, dela den överordnade mappen med grupp A och Lägg till grupp B i den första undermappen.
    
[Sluta dela en fil eller mapp](https://go.microsoft.com/fwlink/?linkid=2008861)
  

