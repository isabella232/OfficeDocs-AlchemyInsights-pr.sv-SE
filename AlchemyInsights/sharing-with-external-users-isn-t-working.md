---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691593"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Åtgärda problem med att dela SharePoint-innehåll med externa användare

Kontrol lera att extern delning är aktiverat för organisationen:
  
1. Gå till [sidan tjänster &amp; -tillägg i administrations centret för Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **webbplatser**.
    
2. Kontrol lera att inställningen är på. Om "endast befintliga externa användare" är markerat kontrollerar du att den externa användaren finns med i Microsoft 365 Admin Center.
    
Kontrol lera att extern delning är aktiverat för webbplatsen. För en klassisk webbplats samling:
  
1. Klicka på **webbplatser**i det nya administrations centret för SharePoint.
    
2. Välj webbplatsen eller platserna och klicka på **delning**i menyfliksområdet.
    
För en grupp webbplats som tillhör en Microsoft 365-grupp eller en kommunikations webbplats:
  
- Dessa nya webbplats typer har samma delnings inställningar som inställning för hela organisationen, såvida inte inställningen för hela organisationen tillåter att filer delas med länkar som inte kräver inloggning. I det här fallet kan webbplatserna dela med nya och befintliga externa användare som loggar in. Om du vill ändra inställningen för vissa webbplatser kan du använda det nya administrations centret för SharePoint eller PowerShell. [Mer information](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Inställningen för extern delning för en webbplats kan vara mer restriktiv än inställningen för hela organisationen, men inte fler tillåtna än inställningen för hela organisationen. 
  

