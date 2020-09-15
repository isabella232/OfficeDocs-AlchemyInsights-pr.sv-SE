---
title: Lägga till externa användare i en distributions grupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663531"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lägga till externa användare i en distributions grupp

Att lägga till en extern kontakt i en distributions grupp är en process i två steg:
  
1. Skapa en e-postkontakt för den externa användaren:
    
    1. Gå till sidan **användare**kontakter i administrations centret  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Välj **Lägg till en kontakt**.
    
    3. Skriv informationen för kontakten och välj **Lägg till**.
    
2. Lägg till e-postkontakten till din DG:
    
    1. Gå till sidan grupper i administrations centret **Groups**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Leta reda på den DG som du vill lägga till den externa användaren i och välj den för att öppna dialog rutan Redigera.
    
    3. På fliken **medlemmar** väljer du **Visa alla och hantera medlemmar**. 
    
    4. Välj **Lägg till medlemmar**.
    
    5. Markera den e-postkontakt som du skapade i föregående steg och välj sedan **Spara**.
    
Om de externa användarna inte kan skicka e-post till DG eller inte ta emot e-post från den här proceduren, kan det bero på att DG är markerat för att endast tillåta e-post från interna användare. Du kan kontrol lera denna konfiguration och åtgärda den enligt anvisningarna [här](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Obs!** De här instruktionerna gäller inte om gruppens typ är "Microsoft 365 Group" i stället för "distribution Group". Om så är fallet kan du lägga till den externa användaren direkt i gruppen från Outlook. Detaljerad information om Microsoft 365-grupp gäster och anvisningar för att lägga till externa gäster finns i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  