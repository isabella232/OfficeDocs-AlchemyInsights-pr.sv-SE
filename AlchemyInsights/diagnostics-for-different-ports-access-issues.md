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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="fcfdf-102">Diagnostik för olika åtkomstproblem med portar</span><span class="sxs-lookup"><span data-stu-id="fcfdf-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="fcfdf-103">Så här löser du olika problem med portåtkomst:</span><span class="sxs-lookup"><span data-stu-id="fcfdf-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="fcfdf-104">Stoppa/avtala den virtuella datorn från portalen, starta om den virtuella maskinerna och testa igen.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="fcfdf-105">Kontrollera den virtuella datorns nätverksinställningar för att fastställa om du har nätverkets säkerhetsgrupper som blockerar trafiken.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="fcfdf-106">Du kan också använda [Network Watcher-verktyget FÖR](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) IP-flödeskontroll för att kontrollera om NSG-blockerar trafik, User-Defined Routes (UDRs) omdirigering av trafiken tillbaka till den lokala ('Default Route' 0.0.0.0/0) eller till ett nätverksverktyg.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="fcfdf-107">Om du fortfarande har problem när du har försökt med stegen ovan anger du namnet på den virtuella datorn och TCP-porten som du försöker skicka e-post på för ytterligare diagnos.</span><span class="sxs-lookup"><span data-stu-id="fcfdf-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="fcfdf-108">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="fcfdf-108">**Recommended Documents**</span></span>

[<span data-ttu-id="fcfdf-109">Begränsningar och rekommendationer för att skicka utgående e-post via port 25</span><span class="sxs-lookup"><span data-stu-id="fcfdf-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)