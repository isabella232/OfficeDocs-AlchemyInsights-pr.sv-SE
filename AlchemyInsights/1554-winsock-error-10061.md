---
title: 1554 Winsock-fel 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492419"
---
# <a name="winsock-error-10061"></a>Winsock-fel 10061

Felet innebär att Office 365 gick inte att upprätta en TCP-socket (anslutning) med målvärden. Den mest troliga orsaken till detta fel är ett problem med konfigurationen av brandväggen. Åtgärda problemet genom att kontrollera inställningarna:
  
- Kontrollera konfigurationen av brandväggen med informationen i [Office 365-adresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Om felet är specifikt till Exchange Online skydd (EOP), bör du tidigare anmälts till en ändring till [Exchange Online skydd IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Kontrollera att porten inte blockering av Internet Service Provider (ISP).
    
- Kontrollera smart värd- och måldator-serverinställningarna i kopplingar.
    
Observera att Office 365 inte blockerar *inkommande* anslutningar på detta sätt. 
  

