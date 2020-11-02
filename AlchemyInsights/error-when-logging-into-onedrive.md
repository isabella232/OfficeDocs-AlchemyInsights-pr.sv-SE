---
title: 0x8004de40-fel när du startar OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823119"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-fel när du startar OneDrive

Om du får ett fel **meddelande när du** loggar in på OneDrive startar du om datorn när du är ansluten till din arbets-eller skol domän. Om du får det här felet efter att du har startat om datorn kan du prova det när du är ansluten till din arbets-eller skol domän:

1. Klicka på Start och skriv **cmd** eller **kommando tolken**  i sökrutan, högerklicka på appen kommando tolken och välj  **Kör som administratör** . Om du uppmanas att ange ett administratörs lösen ord eller en bekräftelse skriver du lösen ordet eller klickar på **Tillåt** .  

2. I kommando tolken skriver du **dsregcmd/Leave**  och väntar på att kommandot ska slutföras. Skriv sedan **dsregcmd/Join** och vänta tills kommandot har slutförts.
3. Starta om datorn.
