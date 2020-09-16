---
title: Logga in i Windows 10 utan lösen ord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719971"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logga in i Windows 10 utan lösen ord

För att undvika att behöva ange ett lösen ord när du startar Windows rekommenderar vi att du använder ett av de säkra inloggnings alternativen för Windows Hello, till exempel en PIN-kod, en ansikts igenkänning eller ett finger avtryck, om det är tillgängligt. Om du vill inaktivera säker inloggning kan du läsa anvisningarna "logga in automatiskt på Windows 10" nedan.

**Säkra Windows Hello-alternativ till konto lösen ordet**

Gå till **inställningar > konton > inloggnings alternativ** (eller klicka [här](ms-settings:signinoptions?activationSource=GetHelp)). Tillgängliga inloggnings alternativ visas. Ett exempel:

![Inloggnings alternativ.](media/sign-in-options.png)

Klicka eller tryck på ett av alternativen för att konfigurera det. Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösen ord. 

**Logga in automatiskt i Windows 10**

**Obs!** automatisk inloggning är bekvämt, men introducerar en säkerhets risk, särskilt om din dator är tillgänglig för flera personer. 

1. Klicka eller tryck på **Start** -knappen i aktivitets fältet.

2. Skriv **netplwiz** och tryck på RETUR för att öppna fönstret användar konton.

3. I **användar konton**klickar du på det konto som du vill logga in automatiskt på när Windows startas.

4. Avmarkera kryss rutan "användare måste ange användar namn och lösen ord för att använda den här datorn".

    ![Användare måste ange ett användar namn och lösen ord.](media/users-must-enter-username.png)

5. Klicka på **OK**. Du uppmanas att ange och bekräfta lösen ordet för det konto som du har valt. Klicka på **OK** för att avsluta. Nästa gång Windows 10 startas loggar det automatiskt in på det konto som du har valt.
