---
title: 2681 Attack Attack i Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545744"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="e389b-102">Attack Attack in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e389b-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="e389b-103">Saknar du Attack Attack?</span><span class="sxs-lookup"><span data-stu-id="e389b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="e389b-104">Attack Attack Attack kräver **Microsoft Defender för Office 365 abonnemang 2** eller Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="e389b-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="e389b-105">Attack Attack Attack **ingår** inte i Microsoft Defender för Office 365 abonnemang 1, Office 365 Enterprise E3 eller andra Microsoft 365-applikationer för affärsverksamhet prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="e389b-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="e389b-106">Det konto du använder för att starta simulerade attacker kräver global administratör eller säkerhetsadministratörsbehörighet och multifaktorautentisering (MFA).</span><span class="sxs-lookup"><span data-stu-id="e389b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="e389b-107">Mer information om attackkraven finns i det [här avsnittet.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="e389b-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="e389b-108">Viktiga saker att veta om **Råstyrt lösenord-attack** simuleringar:</span><span class="sxs-lookup"><span data-stu-id="e389b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="e389b-109">Om målkontot har MFA aktiverat och lösenordet gissades rätt visas inte kontot som komprometterat (den andra autentiseringsfaktorn är ofullständig).</span><span class="sxs-lookup"><span data-stu-id="e389b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="e389b-110">Lösenordsfilen får inte vara större än 10 MB.</span><span class="sxs-lookup"><span data-stu-id="e389b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="e389b-111">Använd ett lösenord per rad och ta med en tom rad (vagnretur) efter det sista lösenordet i listan.</span><span class="sxs-lookup"><span data-stu-id="e389b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="e389b-112">Viktiga saker att veta om **simuleringar av nätfiske:**</span><span class="sxs-lookup"><span data-stu-id="e389b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="e389b-113">Som design kan du inte ange ett anpassat värde för URL för **nätfiskeinloggningsserver.**</span><span class="sxs-lookup"><span data-stu-id="e389b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="e389b-114">Om en mottagare använder [tillägget](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Aktivera rapportmeddelandet för att rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är en simulerad attack).</span><span class="sxs-lookup"><span data-stu-id="e389b-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="e389b-115">Rapporter: När den simulerade attacken är slutförd kan du klicka på **Attackinformation** för att se rapporten.</span><span class="sxs-lookup"><span data-stu-id="e389b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="e389b-116">Detaljerade instruktioner och nya funktioner i Attack Attack Attack finns i [Attack Attack Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="e389b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
