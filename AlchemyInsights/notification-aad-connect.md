---
title: Meddelande om AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037235"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="74254-102">Meddelande om AAD Connect</span><span class="sxs-lookup"><span data-stu-id="74254-102">Notification AAD Connect</span></span>

- <span data-ttu-id="74254-103">Se till att du har behörighet att utföra åtgärden.</span><span class="sxs-lookup"><span data-stu-id="74254-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="74254-104">Globala administratörer har åtkomst som standard.</span><span class="sxs-lookup"><span data-stu-id="74254-104">Global Admins have access by default.</span></span> <span data-ttu-id="74254-105">Du kan dessutom använda rollbaserad [åtkomstkontroll för att delegera](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registreringsbehörighet till deltagare.</span><span class="sxs-lookup"><span data-stu-id="74254-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="74254-106">Se till att de obligatoriska slutpunkterna är aktiverade och inte blockerade på grund av brandväggen.</span><span class="sxs-lookup"><span data-stu-id="74254-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="74254-107">Mer information finns i [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="74254-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="74254-108">Registreringen kan misslyckas på grund av att den utgående kommunikationen görs i SSL-kontrollen av nätverkslagret.</span><span class="sxs-lookup"><span data-stu-id="74254-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="74254-109">Kontrollera att du har verifierat meddelandeinställningarna för Azure AD Connect Health och granska din inställning.</span><span class="sxs-lookup"><span data-stu-id="74254-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="74254-110">Information om hur du konfigurerar meddelandeinställningarna för Azure AD Connect Health-meddelanden finns i den här [guiden.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="74254-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="74254-111">Mer information om AAD Connect Health-synkroniseringsrapporten och hur du laddar ned den finns i [Synkroniseringsrapport för objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="74254-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="74254-112">Om du vill felsöka hälsoaviseringar för AAD Connect följer du felsökningsguiden för varningar om data i [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) och för vanliga frågor och svar finns i Vanliga frågor om installation av [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="74254-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
