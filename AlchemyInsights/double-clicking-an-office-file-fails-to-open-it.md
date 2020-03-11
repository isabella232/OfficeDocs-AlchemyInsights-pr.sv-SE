---
title: Det går inte att öppna den genom att dubbelklicka på en Office-fil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573601"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Det går inte att öppna den genom att dubbelklicka på en Office-fil

När du har dubbelklickat på en Office-fil kan programmet öppnas, men själva filen öppnas inte. Eller så kan du få felet: "Det var ett problem att skicka kommandot till programmet." Det finns många orsaker till detta, men de två vanligaste lösningarna är:

- Inifrån Excel kontrollerar du att Alternativet DDE är avmarkerat. Alternativet kan hittas genom att skapa en ny arbetsbok och sedan välja **Arkiv > Alternativ > Avancerat**. Avmarkera **ignorera andra program som använder DDE (Dynamic Data Exchange) i**avsnittet **Allmänt** .

- Kör en onlinereparation för att återställa standardinställningarna. Klicka på Start-knappen i Windows och sök efter "Kontrollpanelen". Öppna **Kontrollpanelen**och gå till **Program > program och funktioner**. Högerklicka sedan på **Microsoft Office [Version]** och välj **Ändra > Online Repair**.

Om ingen av dessa lösningar fungerar kan en mer komplett lista över lösningar hittas i supportartikeln, [Dubbelklicka på en Office-fil kan inte öppna den](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
