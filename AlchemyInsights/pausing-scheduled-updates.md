---
title: Pausa schemalagda uppdateringar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555991"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="a5f3a-102">Pausa schemalagda uppdateringar</span><span class="sxs-lookup"><span data-stu-id="a5f3a-102">Pausing scheduled updates</span></span>

<span data-ttu-id="a5f3a-103">När ett pauskommando utfärdas bearbetas inte kommandot förrän nästa gång de checkar in på Intune.</span><span class="sxs-lookup"><span data-stu-id="a5f3a-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="a5f3a-104">På grund av detta kan dina enheter ha:</span><span class="sxs-lookup"><span data-stu-id="a5f3a-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="a5f3a-105">Installerade de schemalagda uppdateringarna före incheckningen.</span><span class="sxs-lookup"><span data-stu-id="a5f3a-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="a5f3a-106">Har stängts av när du utfärdade pauskommandot.</span><span class="sxs-lookup"><span data-stu-id="a5f3a-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="a5f3a-107">I det här fallet, när enheterna var påslagna, kan de ha hämtat och installerat de schemalagda uppdateringarna före incheckningen.</span><span class="sxs-lookup"><span data-stu-id="a5f3a-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>