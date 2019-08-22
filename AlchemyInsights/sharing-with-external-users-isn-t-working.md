---
title: Dela med externa användare fungerar inte
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502249"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Åtgärda problem med SharePoint-innehåll med externa användare

Kontrollera extern delning har aktiverats för organisationen:
  
1. Gå till den [tjänster &amp; tillägg sidan i Microsoft 365 administratörscenter](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), och på **platser**.
    
2. Kontrollera att inställningen är ”on”. Om ”endast befintliga externa användare” är markerad, kontrollera att den externa användaren finns med i Microsoft 365 administratörscenter.
    
Kontrollera att externa dela den aktiverad för webbplatsen. För en klassisk webbplatssamling:
  
1. Klicka på **webbplatser**i nya SharePoint administratörscenter, i den vänstra rutan.
    
2. Markera den eller de platser och klicka på **Dela**på menyfliken.
    
För en gruppwebbplats som hör till en grupp i Office 365, eller en webbplats för kommunikation:
  
- Dessa nya typer av webbplatsen har samma delning inställning som inställning för hela organisationen om inställningen hela organisationen kan dela filer med hjälp av länkar som inte kräver inloggning. I det här fallet att webbplatser delar med nya och befintliga externa användare som loggar in. Använd nya SharePoint administratörscenter eller PowerShell om du vill ändra inställningen för specifika platser. [Läs mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Inställningen för extern delning för en webbplats kan vara mer restriktiva än inställningarna hela organisationen, men inte mer tillåtna än inställningen för hela organisationen. 
  

