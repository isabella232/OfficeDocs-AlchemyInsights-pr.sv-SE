---
title: Administrationscenter för Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826397"
---
# <a name="teams-admin-center"></a><span data-ttu-id="74c8b-102">Administrationscenter för Teams</span><span class="sxs-lookup"><span data-stu-id="74c8b-102">Teams Admin Center</span></span>

<span data-ttu-id="74c8b-103">Lär dig mer om hur du hanterar Teams med [Administrationscenter för Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="74c8b-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="74c8b-104">Om du saknar åtkomst till Administrationscenter för Teams kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="74c8b-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="74c8b-105">Att du har tillåtit lämpliga [IP-adresser och URL:er för Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alla perimeterenheter (brandvägg osv.) eller i brandväggsreglerna på din lokala dator.</span><span class="sxs-lookup"><span data-stu-id="74c8b-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="74c8b-106">Att inloggningen du använder för åtkomst till Administrationscenter för Teams matchar ditt användarnamn som visas i [administrationsportalen för Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="74c8b-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="74c8b-107">Om användarna inte visas i Administrationscenter för Teams kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="74c8b-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="74c8b-108">Har du skapat användare eller tilldelat licenser under de senaste 24 timmarna?</span><span class="sxs-lookup"><span data-stu-id="74c8b-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="74c8b-109">Se till att vänta minst 24 timmar innan du skapar ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="74c8b-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="74c8b-110">Har du tilldelat lämpliga licenser?</span><span class="sxs-lookup"><span data-stu-id="74c8b-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="74c8b-111">Om du har en lokal Active Directory kontrollerar du att värdet för [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) eller SIP-adressen i fältet ProxyAddresses i din lokala Active Directory är unikt och formatet matchar **sip:** Användarens användarnamn från administrationscentret för [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="74c8b-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="74c8b-112">Om du har för avsikt att behålla en Skype för företag – Server-distribution och låta användarna vara lokalt uppkopplade och online: följ **"Konfigurera hybrid** med Teams och Skype för företag – Online" i Skype för företag – Server-kontrollpanelen och flytta användare online.</span><span class="sxs-lookup"><span data-stu-id="74c8b-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
