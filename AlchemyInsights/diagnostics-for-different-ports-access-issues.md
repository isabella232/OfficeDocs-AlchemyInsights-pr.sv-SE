---
title: Diagnostik för olika åtkomstproblem med portar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030920"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostik för olika åtkomstproblem med portar

Så här löser du olika problem med portåtkomst:

1. Stoppa/avtala den virtuella datorn från portalen, starta om den virtuella maskinerna och testa igen. 
2. Kontrollera den virtuella datorns nätverksinställningar för att fastställa om du har nätverkets säkerhetsgrupper som blockerar trafiken. Du kan också använda [Network Watcher-verktyget FÖR](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) IP-flödeskontroll för att kontrollera om NSG-blockerar trafik, User-Defined Routes (UDRs) omdirigering av trafiken tillbaka till den lokala ('Default Route' 0.0.0.0/0) eller till ett nätverksverktyg.
Om du fortfarande har problem när du har försökt med stegen ovan anger du namnet på den virtuella datorn och TCP-porten som du försöker skicka e-post på för ytterligare diagnos.

**Rekommenderade dokument**

[Begränsningar och rekommendationer för att skicka utgående e-post via port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)