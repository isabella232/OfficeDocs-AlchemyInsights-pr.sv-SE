---
title: 0x8004de40 vid start av OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946597"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 vid start av OneDrive

Om ett felmeddelande visas när **0x8004de40** loggar in i OneDrive startar du om datorn medan du är ansluten till din arbets- eller skoldomän. Om det här felmeddelandet visas när du har startat om kan du försöka med det här när du är ansluten till din arbets- eller skoldomän:

1. Klicka på Start och skriv **cmd** eller **kommandotolken** i sökrutan, högerklicka på kommandotolken och välj **Kör som administratör.** Om du uppmanas att ange ett administratörslösenord eller att bekräfta skriver du lösenordet eller klickar på **Tillåt**.  

2. I fönstret Kommandotolken skriver du **dsregcmd /leave**  och väntar tills kommandot har slutförts. Skriv **sedan dsregcmd /join** och vänta tills kommandot har slutförts.
3. Starta om datorn.
