---
title: 1554 Winsock-fel 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698880"
---
# <a name="winsock-error-10061"></a>Winsock-fel 10061

Den här felkoden innebär att Microsoft inte kunde upprätta en TCP-socket (anslutning) med mål värden. Den mest sannolika orsaken till det här felet är ett problem med din brand Väggs konfiguration. Åtgärda problemet genom att kontrol lera följande:

- Kontrol lera din brand Väggs konfiguration med informationen i [Microsoft 365 URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Om felet är specifikt för Exchange Online Protection (EOP), bör du tidigare meddelas om [Exchange Online Protection IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Kontrol lera att Internet leverantören inte blockerar porten.

- Kontrol lera inställningarna för smart värd och mål server i dina kontakter.

Observera att Microsoft 365 inte blockerar *inkommande* anslutningar på det här sättet.
