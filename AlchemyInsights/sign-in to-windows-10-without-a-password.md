---
title: Logga in på Windows 10 utan att använda ett lösenord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588298"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logga in på Windows 10 utan att använda ett lösenord

För att undvika att behöva skriva ett lösenord vid start av Windows rekommenderar vi att du använder något av alternativen för säker inloggning i Windows Hello, till exempel en PIN-kod, ansiktsigenkänning eller fingeravtryck, om tillgängligt. Om du verkligen vill inaktivera säker inloggning läser du instruktionerna "Logga automatiskt in i Windows 10" nedan.

**Säkra Windows Hello-alternativ till kontolösenordet**

Gå till **Inställningar > konton > inloggningsalternativ** (eller klicka [här).](ms-settings:signinoptions?activationSource=GetHelp) Tillgängliga inloggningsalternativ visas. Till exempel:

![Inloggningsalternativ.](media/sign-in-options.png)

Klicka eller tryck på något av alternativen för att konfigurera det. Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösenord. 

**Logga in automatiskt i Windows 10**

**Automatisk**inloggning är praktiskt, men introducerar en säkerhetsrisk, särskilt om datorn är tillgänglig för flera personer. 

1. Klicka eller tryck på **Start-knappen** i Aktivitetsfältet.

2. Skriv **netplwiz** och tryck på Retur-tangenten för att öppna fönstret Användarkonton.

3. I **Användarkonton**klickar du på det konto som du vill logga in automatiskt på när Windows startar.

4. Avmarkera kryssrutan "Användare måste ange ett användarnamn och lösenord för att använda den här datorn".

    ![Användare måste ange ett användarnamn och lösenord alternativ.](media/users-must-enter-username.png)

5. Klicka på **OK**. Du kommer att bli ombedd att ange och bekräfta lösenordet för det valda kontot. Klicka på **OK** för att avsluta. Nästa gång Windows 10 startar loggas det automatiskt in på det konto du valde.
