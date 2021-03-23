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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036807"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostik för olika åtkomstproblem med portar

Så här löser du olika problem med portåtkomst:

1. Stoppa/avtala den virtuella datorn från portalen, starta om den virtuella maskinerna och testa igen. 
2. Kontrollera den virtuella datorns nätverksinställningar för att fastställa om du har nätverkets säkerhetsgrupper som blockerar trafiken. Du kan också använda [Network Watcher-verktyget FÖR](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) IP-flödeskontroll för att kontrollera om NSG-blockerar trafik, User-Defined Routes (UDRs) omdirigering av trafiken tillbaka till den lokala ('Default Route' 0.0.0.0/0) eller till ett nätverksverktyg.
Om du fortfarande har problem när du har försökt med stegen ovan anger du namnet på den virtuella datorn och TCP-porten som du försöker skicka e-post på för ytterligare diagnos.

**Rekommenderade dokument**

[Begränsningar och rekommendationer för att skicka utgående e-post via port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)