---
title: Logga in på Windows 10 utan att använda ett lösenord
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830564"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logga in på Windows 10 utan att använda ett lösenord

Om du vill undvika att behöva ange ett lösenord vid start av Windows rekommenderar vi att du använder ett av de säkra inloggningsalternativen i Windows Hello, till exempel pin-kod, ansiktsigenkänning eller fingeravtryck, om sådana finns tillgängliga. Om du verkligen vill inaktivera säker inloggning kan du läsa instruktionerna "Logga in automatiskt på Windows 10" nedan.

**Säkra Windows Hello-alternativ till kontolösenordet**

Gå till **Inställningar > Konton > Inloggningsalternativ (eller** klicka [här](ms-settings:signinoptions?activationSource=GetHelp)). Tillgängliga inloggningsalternativ visas. Till exempel:

![Inloggningsalternativ.](media/sign-in-options.png)

Konfigurera det genom att klicka eller trycka på något av alternativen. Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösenord. 

**Logga in automatiskt på Windows 10**

**Obs!** Automatisk inloggning är praktiskt, men innebär en säkerhetsrisk, särskilt om datorn är tillgänglig för flera personer. 

1. Klicka eller tryck på **Start-knappen** i Aktivitetsfältet.

2. Skriv **netplwiz** och tryck på Retur för att öppna fönstret Användarkonton.

3. I **Användarkonton** klickar du på det konto som du vill logga in på automatiskt när Windows startar.

4. Avmarkera kryssrutan "Användare måste ange ett användarnamn och lösenord för att kunna använda den här datorn".

    ![Användarna måste ange ett alternativ för användarnamn och lösenord.](media/users-must-enter-username.png)

5. Klicka på **OK**. Du uppmanas att ange och bekräfta lösenordet för det konto som du valt. Slutför genom att klicka på **OK.** Nästa gång Windows 10 startar loggas det automatiskt in på det konto som du har valt.
