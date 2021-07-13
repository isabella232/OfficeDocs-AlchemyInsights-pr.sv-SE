---
title: Domänstatus – Inga tjänster har markerats
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389199"
---
# <a name="domain-status---no-services-selected"></a>Domänstatus – Inga tjänster har markerats

**Inga tjänster valda** innebär att du inte har valt några Microsoft 365-tjänster som Exchange Online, Skype för företag eller Intune eller Hantering av mobila enheter för Microsoft 365 som ska användas med din egen domän. Om du använder Exchange hybridfiltrering (Exchange lokalt med Exchange Online) eller extern skräppostfiltrering med Exchange och inga andra Microsoft-tjänster kan du ignorera det här meddelandet. Status för domänhälsa är endast tillgänglig för domäner som är anslutna direkt till tjänsten.

Så här väljer du tjänster för domänen:

1. I **Inställningar**  >  [**Domäner**](https://admin.microsoft.com/Adminportal/Home)markerar du kryssrutan bredvid domänen med statusmeddelandet **Inga tjänster markerat.**
1. Välj **Hantera DNS för** att starta domäninstallationsguiden.
    - Om du väljer **Lägg till dina egna DNS-poster** ska du se till att välja en tjänst när du uppmanas att göra det. Fler tjänster kan vara tillgängliga under **Avancerade alternativ.**
    - Om du väljer **Låt Microsoft lägga till dina DNS-poster** eller **Fler** alternativ Konfigurera onlinetjänsterna åt mig föreslås alla tillgängliga tjänster  >   och väljs automatiskt.
1. Fortsätt genom guiden för att slutföra DNS-installationen och tjänstalternativen.
 
Mer hjälp med att konfigurera din domän finns i Lägga [till DNS-poster för att ansluta din domän.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

