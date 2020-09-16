---
title: Felsöka ljud problem i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750361"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Felsöka ljud problem i Windows 10

**Köra fel sökaren för ljud**

1.  Öppna [fel söknings inställningar](ms-settings:troubleshoot).

2.  Välj **spela upp ljud**  >  **kör fel sökaren**.

**Ange standardenhet**

Om du ansluter till en ljuden het med USB eller HDMI kan du behöva ange enheten som standard:

1. Öppna **Start**  >  **ljud**och välj sedan **ljud** eller **ändra system ljud** i resultat listan.

2.  Välj en enhet på fliken **uppspelning** och välj **Ange standard**och sedan **OK**.

**Kontrol lera kablar, volym, högtalare och hörlurar**

1. Kontrol lera att du har kablar och hörlurs samtal och se till att de är anslutna till rätt uttag.

2. Kontrol lera energi-och volym nivåerna och prova att aktivera alla volym kontroller.

3. Vissa högtalare och appar har sina egna volym kontroller; Du kanske måste kontrol lera dem så att de är på rätt nivå.

4. Prova att ansluta med en annan USB-port.

**Obs!** kom ihåg att dina högtalare kanske inte fungerar när hörlurarna ansluts.

**Kontrol lera enhets hanteraren**

Så här kontrollerar du att driv rutinerna är uppdaterade:

1. Välj **Start**, Skriv **enhets hanteraren**och välj sedan **enhets hanteraren** i resultat listan.

2. Välj ljud kortet under **ljud-, video-och spel enheter**, öppna det, Välj fliken **driv rutin** och välj **Uppdatera driv rutin**.

**Obs!** om Windows inte hittar en ny driv rutin kan du leta efter en på tillverkarens webbplats och följa deras instruktioner.

**Installera om driv rutinen**

Om du inte kan uppdatera via enhets hanteraren eller hitta en ny driv rutin på tillverkarens webbplats kan du prova följande:

1. Högerklicka på (eller håll ned) ljud driv rutinen i enhets hanteraren och välj **Avinstallera**. Starta om enheten så försöker Windows installera om driv rutinen.

2. Om det inte fungerar att installera om driv rutinen kan du försöka använda den allmänna ljud driv rutinen som medföljer Windows. I enhets hanteraren högerklickar du på (eller trycker på och håller ned) ljud driv rutinen > **Uppdatera driv**rutin  >  **Bläddra på den här datorn efter driv**rutiner kan du välja  >  **från en lista på**driv rutinen på datorn, välja HD- **ljudenhet**, välja **Nästa**och följa anvisningarna för att installera den.
