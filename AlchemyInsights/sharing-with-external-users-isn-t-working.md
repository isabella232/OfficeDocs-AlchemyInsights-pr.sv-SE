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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910384"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Åtgärda problem med att SharePoint innehåll med externa användare

Kontrollera att extern delning är aktiverat för din organisation:
  
1. Gå till [sidan &amp; Tjänster-tillägg i Administrationscenter för Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **Webbplatser.**
    
2. Kontrollera att inställningen är "På". Om "Endast befintliga externa användare" är markerat kontrollerar du att den externa användaren står med i listan Administrationscenter för Microsoft 365.
    
Kontrollera att extern delning är aktiverat för webbplatsen. För en klassisk webbplatssamling:
  
1. Klicka på SharePoint i den vänstra rutan i det nya **administrationscentret.**
    
2. Markera webbplatsen eller webbplatserna och klicka på Delning i **menyfliksområdet.**
    
För en gruppwebbplats som tillhör en Microsoft 365 grupp eller en kommunikationswebbplats:
  
- De här nya webbplatstyperna har samma delningsinställning som inställningen för hela organisationen, om inte inställningen för hela organisationen tillåter delning av filer med länkar som inte kräver inloggning. I det här fallet tillåter webbplatserna delning med nya och befintliga externa användare som loggar in. Om du vill ändra inställningen för specifika webbplatser använder du det SharePoint administrationscentret eller PowerShell. [Mer information](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Inställningen för extern delning för alla webbplatser kan vara mer restriktiv än den organisationsomfattande inställningen, men inte mer tillåtande än inställningen för hela organisationen. 
  

