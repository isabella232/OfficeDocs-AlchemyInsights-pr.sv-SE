---
title: 1554 Winsock fel 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766187"
---
# <a name="winsock-error-10061"></a>Winsock fel 10061

Den här felkoden innebär att Microsoft inte kunde upprätta en TCP-socket (anslutning) med målvärden. Den troligaste orsaken till det här felet är ett problem med brandväggskonfigurationen. Kontrollera följande inställningar för att åtgärda problemet:

- Verifiera brandväggskonfigurationen med informationen i [Microsoft 365-URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Om felet är specifikt för Exchange Online Protection (EOP) bör du tidigare ha meddelats om en ändring av [EXCHANGE Online Protection IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontrollera att Internet-leverantören inte blockerar porten.

- Verifiera inställningarna för den smarta värden och målservern i kontakterna.

Observera att Microsoft 365 inte blockerar *inkommande* anslutningar på detta sätt.
