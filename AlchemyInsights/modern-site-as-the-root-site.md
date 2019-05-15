---
title: Modern webbplats som rotwebbplatsen
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057783"
---
# <a name="modern-site-as-root-site"></a>Modern webbplats som rotplats

[Målet Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) -kunder kan nu modern kommunikations webbplats erfarenhet på klassiska rotwebbplatsen för sina SharePoint-innehavare.

Den här funktionen kan aktiveras genom att köra en enkel PowerShell-cmdlet. I PowerShell-kommandon att utföra har rotplatsen en ny hemsida för kommunikation webbplats. Information om krav för PowerShell-cmdlet och funktionen finns i artikeln [Aktivera SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Vi kommer gradvis rullande detta, av som standard till riktade Release kunder i tidiga maj 2019 och rulle ut blir tillgänglig över hela världen i slutet av juni 2019. Fortsätta att referera till [Meddelandecenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) för andra nya funktioner med Modern. 

**Viktigt**: ta inte bort klassiska rot-webbplats om du vill skapa en webbplats för modern kommunikation. Detta stöds inte av Microsoft. Ta bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen inte tillgänglig för alla användare förrän du återställer en webbplats eller skapa en ny webbplats med samma URL. 
 
 