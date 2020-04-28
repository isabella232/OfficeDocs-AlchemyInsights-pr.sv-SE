---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913020"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Åtgärda problem med att dela SharePoint-innehåll med externa användare

Kontrollera att extern delning är aktiverat för din organisation:
  
1. Gå till [ &amp; sidan Tjänster-tillägg i administrationscentret för Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **Webbplatser**.
    
2. Kontrollera att inställningen är aktiverad. Om "Endast befintliga externa användare" är markerat kontrollerar du att den externa användaren finns med i Microsoft 365-administrationscentret.
    
Kontrollera att extern delning är aktiverat för webbplatsen. För en klassisk webbplatssamling:
  
1. Klicka på **webbplatser**i det nya administrationscentret för SharePoint i det nya administrationscentret för SharePoint.
    
2. Markera webbplatsen eller webbplatserna och klicka på **Dela**i menyfliksområdet .
    
För en gruppwebbplats som tillhör en Microsoft 365-grupp eller en kommunikationswebbplats:
  
- Dessa nya webbplatstyper har samma delningsinställning som din organisationsomfattande inställning, såvida inte inställningen för hela organisationen tillåter delning av filer med hjälp av länkar som inte kräver inloggning. I det här fallet tillåter webbplatserna delning med nya och befintliga externa användare som loggar in. Om du vill ändra inställningen för specifika webbplatser använder du det nya Administrationscentret för SharePoint eller PowerShell. [Mer information](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Inställningen för extern delning för en webbplats kan vara mer restriktiv än din organisationsomfattande inställning, men inte mer tillåtande än den organisationsomfattande inställningen. 
  

