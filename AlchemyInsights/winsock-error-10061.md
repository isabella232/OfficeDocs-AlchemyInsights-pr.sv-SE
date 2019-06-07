---
title: 1554 Winsock-fel 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757128"
---
# <a name="winsock-error-10061"></a>Winsock-fel 10061

Felet innebär att Office 365 gick inte att upprätta en TCP-socket (anslutning) med målvärden. Den mest troliga orsaken till detta fel är ett problem med konfigurationen av brandväggen. Åtgärda problemet genom att kontrollera inställningarna:

- Kontrollera konfigurationen av brandväggen med informationen i [Office 365-adresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Om felet är specifikt till Exchange Online skydd (EOP), bör du tidigare anmälts till en ändring till [Exchange Online skydd IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontrollera att porten inte blockering av Internet Service Provider (ISP).

- Kontrollera smart värd- och måldator-serverinställningarna i kopplingar.

Observera att Office 365 inte blockerar *inkommande* anslutningar på detta sätt.
