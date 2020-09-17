---
title: Om du dubbelklickar på en Office-fil öppnas inte den
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812097"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Om du dubbelklickar på en Office-fil öppnas inte den

När du dubbelklickar på en Office-fil kan programmet öppnas, men själva filen öppnas inte. Eller så får du fel meddelandet "ett problem uppstod när du skickade kommandot till programmet". Det finns många orsaker till det, men de två vanligaste lösningarna är:

- I Excel kontrollerar du att DDE-alternativet inte är markerat. Du kan hitta alternativet genom att skapa en ny arbets bok och sedan välja **alternativ för > > Avancerat**. I avsnittet **Allmänt** avmarkerar du **Ignorera andra program som använder DDE (Dynamic Data Exchange)**.

- Kör en online-reparation för att återställa standardinställningarna. Klicka på Start-knappen i Windows och Sök efter "kontroll panelen". Öppna **kontroll panelen**och gå till **program > program och funktioner**. Högerklicka sedan på **Microsoft Office [version]** och välj **ändra > online-reparation**.

Om ingen av dessa lösningar fungerar, en mer fullständig lista över lösningar finns i Support artikeln kan du [dubbelklicka på en Office-fil för att öppna den](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
