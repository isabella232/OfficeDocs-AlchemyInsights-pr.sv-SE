---
title: Problem med AAD Connect-hälsa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483121"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="6d489-102">Problem med AAD Connect-hälsa</span><span class="sxs-lookup"><span data-stu-id="6d489-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="6d489-103">Kontrollera att du har behörighet att utföra åtgärden.</span><span class="sxs-lookup"><span data-stu-id="6d489-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="6d489-104">Globala administratörer har åtkomst som standard.</span><span class="sxs-lookup"><span data-stu-id="6d489-104">Global Admins have access by default.</span></span> <span data-ttu-id="6d489-105">Du kan dessutom använda rollbaserad åtkomstkontroll [för att delegera](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registreringsbehörighet för deltagare.</span><span class="sxs-lookup"><span data-stu-id="6d489-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="6d489-106">Se till att de slutpunkter som krävs är aktiverade och inte blockerade på grund av brandväggen.</span><span class="sxs-lookup"><span data-stu-id="6d489-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="6d489-107">Mer information finns i [kraven.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="6d489-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="6d489-108">Registreringen kan misslyckas på grund av att den utgående kommunikationen infaller på SSL-kontrollen av nätverkslagret.</span><span class="sxs-lookup"><span data-stu-id="6d489-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="6d489-109">Kontrollera att du har verifierat meddelandeinställningarna för Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="6d489-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="6d489-110">Granska inställningen.</span><span class="sxs-lookup"><span data-stu-id="6d489-110">Please review your setting.</span></span> <span data-ttu-id="6d489-111">Den [här](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) guiden hjälper dig att förstå hur du konfigurerar meddelandeinställningarna för hälsomeddelanden i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6d489-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="6d489-112">Mer information om AAD Connect Health-synkroniseringsrapporten och hur du laddar ned den finns i [synkroniseringsrapporten för objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="6d489-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="6d489-113">Om du vill felsöka AAD Connect Health-varningar följer du felsökningsguiden för [AAD Connect Health-varningar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) om data freshness och för vanliga frågor, se Vanliga frågor om [AAD Connect Health-installationen.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="6d489-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
