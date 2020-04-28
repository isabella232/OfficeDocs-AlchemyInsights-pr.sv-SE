---
title: Lägga till externa användare i en distributionsgrupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910950"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lägga till externa användare i en distributionsgrupp

Att lägga till en extern kontakt i en distributionsgrupp (GD) är en tvåstegsprocess:
  
1. Skapa en e-postkontakt för den externa användaren:
    
    1. Gå till sidan[Användares kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i **administrationscentret.** >  
    
    2. Välj **Lägg till en kontakt**.
    
    3. Skriv informationen för kontakten och välj **Lägg till**.
    
2. Lägg till e-postkontakten i gd:
    
    1. Gå till sidan **Gruppergrupper** > [i](https://admin.microsoft.com/adminportal/home#/groups) administrationscentret. 
    
    2. Leta reda på det DG som du vill lägga till den externa användaren i och markera det för att öppna redigeringsdialogrutan.
    
    3. På fliken **Medlemmar** väljer du **Visa alla och hanterar medlemmar**. 
    
    4. Välj **Lägg till medlemmar**.
    
    5. Markera den e-postkontakt som du skapade i föregående steg och välj sedan **Spara**.
    
Om dina externa användare efter att ha följt dessa steg inte kan skicka e-post till GD eller inte får e-postmeddelanden från det, kan det vara så att GD är markerat för att endast tillåta e-postmeddelanden från interna användare. Du kan kontrollera den här konfigurationen och åtgärda den efter anvisningarna [här](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Anm.:** De här instruktionerna gäller inte om gruppens typ är "Microsoft 365-grupp" i stället för "Distributionsgrupp". Om så är fallet kan du lägga till den externa användaren direkt i gruppen från Outlook. Detaljerad information om Microsoft 365 Groups gäster samt instruktioner för att lägga till externa gäster finns i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  