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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813670"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 vid start av OneDrive

Om ett felmeddelande visas när **0x8004de40** loggar in på OneDrive startar du om datorn medan du är ansluten till din arbets- eller skoldomän. Om det här felmeddelandet visas när du har startat om kan du försöka med det här när du är ansluten till din arbets- eller skoldomän:

1. Klicka på Start och skriv **cmd** eller **kommandotolken** i sökrutan, högerklicka på kommandotolken och välj **Kör som administratör.** Om du uppmanas att ange ett administratörslösenord eller att bekräfta skriver du lösenordet eller klickar på **Tillåt**.  

2. I fönstret Kommandotolken skriver du **dsregcmd /leave**  och väntar tills kommandot har slutförts. Skriv **sedan dsregcmd /join** och vänta tills kommandot har slutförts.
3. Starta om datorn.
