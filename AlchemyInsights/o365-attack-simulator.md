---
title: 2681 Attack Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506756"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="7edcf-102">Attack Simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7edcf-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="7edcf-103">Saknar du Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="7edcf-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="7edcf-104">Attack Simulator kräver **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="7edcf-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="7edcf-105">Attack Simulator ingår **inte** i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps for business-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="7edcf-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="7edcf-106">Kontot som du använder för att starta simulerade attacker kräver globala administratörs- eller säkerhetsadministratörsbehörigheter och MFA (Multifaktorautentisering).</span><span class="sxs-lookup"><span data-stu-id="7edcf-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="7edcf-107">Mer information om attacksimulatorkrav finns i [det här avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="7edcf-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="7edcf-108">Viktiga saker att veta om **Brute Force Password** attack simuleringar:</span><span class="sxs-lookup"><span data-stu-id="7edcf-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="7edcf-109">Om målkontot har MFA aktiverat och lösenordet gissades korrekt visas kontot inte som komprometterat (den andra autentiseringsfaktorn kommer att vara ofullständig).</span><span class="sxs-lookup"><span data-stu-id="7edcf-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="7edcf-110">Lösenordsfilen får inte vara större än 10 MB.</span><span class="sxs-lookup"><span data-stu-id="7edcf-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="7edcf-111">Använd ett lösenord per rad och inkludera en tom rad (vagnretur) efter det sista lösenordet i listan.</span><span class="sxs-lookup"><span data-stu-id="7edcf-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="7edcf-112">Viktiga saker att veta om **Spear Phishing** bifoga simuleringar:</span><span class="sxs-lookup"><span data-stu-id="7edcf-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="7edcf-113">Avsiktligt kan du inte ange ett anpassat värde för **webbloggningsserverns URL**.</span><span class="sxs-lookup"><span data-stu-id="7edcf-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="7edcf-114">Om en mottagare använder [tillägget Aktivera rapportmeddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) för att rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är en simulerad attack).</span><span class="sxs-lookup"><span data-stu-id="7edcf-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="7edcf-115">Rapporter: När den simulerade attacken är klar kan du klicka på **Attackinformation** för att se rapporten.</span><span class="sxs-lookup"><span data-stu-id="7edcf-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="7edcf-116">Detaljerade instruktioner och nya funktioner i Attack Simulator finns [i Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="7edcf-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
