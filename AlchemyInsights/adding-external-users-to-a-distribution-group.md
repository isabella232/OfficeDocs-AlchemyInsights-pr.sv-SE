---
title: Lägga till externa användare till en distributionsgrupp
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494545"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lägga till externa användare till en distributionsgrupp?

Lägga till en extern kontakt till en Distribution grupp (GD) är en process i steg 2:
  
1. Skapa en e-kontakt för externa användare:
    
    1. Gå till **användare**i administratörscenter, > [sidan](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Välj **Lägg till en kontakt**.
    
    3. Ange information om kontakten och välj **Lägg till**.
    
2. Lägg till e-kontakt i din DG:
    
    1. Gå till **grupper**i administratörscenter, > [grupper](https://admin.microsoft.com/adminportal/home#/groups) -sidan. 
    
    2. Hitta DG som du vill lägga till den externa användaren till och markera den för att öppna dialogrutan Redigera.
    
    3. Välj **Visa alla och hantera medlemmar**på fliken **medlemmar** . 
    
    4. Välj **Lägg till medlemmar**.
    
    5. Välj e-kontakt som du skapade i föregående steg och välj sedan **Spara**.
    
Om efter följande externa användare kan inte skicka e-post till GD eller inte ta emot e-postmeddelanden från den, kan det bero på att GD har markerats för att endast tillåta e-postmeddelanden från interna användare. Du kan kontrollera konfigurationen och åtgärda det följa instruktionerna [här](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Observera:** Dessa instruktioner gäller inte om din grupp är ”Office 365-grupp” i stället för ”distributionsgrupp”. Om så är fallet kan du lägga till den externa användaren direkt till gruppen från Outlook. Mer information om Office 365-grupper gäster och instruktioner för att lägga till externa gäster kan hittas i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  