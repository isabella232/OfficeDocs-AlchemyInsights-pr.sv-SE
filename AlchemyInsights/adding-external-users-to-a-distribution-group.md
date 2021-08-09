---
title: Lägga till externa användare i en distributionsgrupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934851"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lägga till externa användare i en distributionsgrupp

Att lägga till en extern kontakt i en distributionsgrupp (DG) är en process i två steg:
  
1. Skapa en e-postkontakt för den externa användaren:
    
    1. Gå till sidan Användare kontakter **i**  >  [administrationscentret.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Välj **Lägg till en kontakt**.
    
    3. Skriv informationen för kontakten och välj Lägg **till**.
    
2. Lägg till e-postkontakten i din DG:
    
    1. Gå till sidan Grupper i **administrationscentret.**  >  [](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Leta reda på DG som du vill lägga till den externa användaren i och markera den för att öppna redigeringsdialogrutan.
    
    3. På fliken **Medlemmar** väljer du **Visa alla och hanterar medlemmar.** 
    
    4. Välj **Lägg till medlemmar.**
    
    5. Välj den e-postkontakt du skapade i föregående steg och välj sedan **Spara**.
    
Om externa användare inte kan skicka e-postmeddelanden till DG eller inte kan ta emot e-postmeddelanden från den när de har följt de här stegen kan det vara så att DG har markerats för att endast tillåta e-post från interna användare. Du kan kontrollera den här konfigurationen och åtgärda den med anvisningarna [här](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Obs!** De här instruktionerna gäller inte om gruppens typ är "Microsoft 365" i stället för "Distributionsgrupp". Om så är fallet kan du lägga till den externa användaren direkt i gruppen från Outlook. Detaljerad information om Microsoft 365 grupper och anvisningar för att lägga till externa gäster finns i den [här artikeln.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  