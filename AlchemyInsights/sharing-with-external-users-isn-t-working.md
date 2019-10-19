---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502249"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Åtgärda problem med att dela SharePoint-innehåll med externa användare

Kontrollera att extern delning är aktiverat för din organisation:
  
1. Gå till [sidan tjänster &amp; -tillägg i Microsoft 365 administratörscenter](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **platser**.
    
2. Kontrollera att inställningen är på. Om "endast befintliga externa användare" är markerad, kontrollera att den externa användaren finns med i Microsoft 365 administratörscenter.
    
Kontrollera att extern delning är aktiverad för webbplatsen. För en klassisk webbplatssamling:
  
1. Klicka på **platser**i det vänstra fönstret i det nya administrationscentret för SharePoint.
    
2. Markera webbplatsen eller platserna och klicka på **delning**i menyfliksområdet.
    
För en gruppwebbplats som tillhör en Office 365-grupp eller en kommunikations plats:
  
- De här nya webbplats typerna har samma delningsinställning som din organisationsomfattande inställning, såvida inte inställningen för hela organisationen tillåter delning av filer med länkar som inte kräver inloggning. I det här fallet tillåter webbplatserna delning med nya och befintliga externa användare som loggar in. Om du vill ändra inställningen för specifika webbplatser använder du det nya SharePoint Admin Center eller PowerShell. [Läs mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Den externa delningsinställningen för en webbplats kan vara mer restriktiv än inställningen för hela organisationen, men inte mer tillåtande än inställningen för hela organisationen. 
  

