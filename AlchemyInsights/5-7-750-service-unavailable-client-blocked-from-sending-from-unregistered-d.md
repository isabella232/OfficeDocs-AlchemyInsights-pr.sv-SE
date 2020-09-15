---
title: 1048 5.7.750-tjänsten är inte tillgänglig. Klienten hindrades från att skicka från oregistrerade domäner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664260"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="31ece-103">5.7.750-klienten hindrades från att skicka från oregistrerad domän</span><span class="sxs-lookup"><span data-stu-id="31ece-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="31ece-104">Felet inträffar när en stor mängd meddelanden skickas från domäner som inte är etablerade i klient organisationen (läggs till som godkända domäner och verifierade).</span><span class="sxs-lookup"><span data-stu-id="31ece-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="31ece-105">Du kan undvika det här felet genom att använda en certifikatbaserad mail-baserad e-postkoppling där certifikatets domän är en etablerad domän, eller så kan du etablera alla sändande domäner.</span><span class="sxs-lookup"><span data-stu-id="31ece-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
