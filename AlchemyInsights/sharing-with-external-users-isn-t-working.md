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
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369516"
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
  

