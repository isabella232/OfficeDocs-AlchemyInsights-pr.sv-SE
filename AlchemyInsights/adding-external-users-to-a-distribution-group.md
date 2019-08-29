---
title: Lägga till externa användare i en distributionsgrupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660810"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lägga till externa användare i en distributionsgrupp

Att lägga till en extern kontakt i en distributionsgrupp (DG) är en tvåstegsprocess:
  
1. Skapa en e-postkontakt för den externa användaren:
    
    1. Gå till sidan **användare** > [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i administratörscenter. 
    
    2. Välj **Lägg till en kontakt**.
    
    3. Ange informationen för din kontakt och välj **Lägg till**.
    
2. Lägg till e-postkontakten i ditt generaldirektorat:
    
    1. I administratörscenter går du till sidan **grupper** > [grupper](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Leta upp den DG du vill lägga till den externa användaren till och välj den för att öppna dialogrutan Redigera.
    
    3. På fliken **medlemmar** väljer du **Visa alla och hantera medlemmar**. 
    
    4. Välj **Lägg till medlemmar**.
    
    5. Välj den e-postkontakt du skapade i föregående steg och välj sedan **Spara**.
    
Om du efter att följa dessa steg dina externa användare inte kan skicka e-post till DG eller inte ta emot e-post från den, kan det vara så att DG är märkt att bara tillåta e-post från interna användare. Du kan kontrollera den här konfigurationen och åtgärda det genom att följa anvisningarna [här](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Anmärkning:** De här anvisningarna gäller inte om gruppens typ är "Office 365-grupp" i stället för "distributionsgrupp". Om så är fallet kan du lägga till den externa användaren direkt till gruppen från Outlook. Detaljerad information om Office 365 grupper gäster samt instruktioner för att lägga till externa gäster finns i [denna artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  