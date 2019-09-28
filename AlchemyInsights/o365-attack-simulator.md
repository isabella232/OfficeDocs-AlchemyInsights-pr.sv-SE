---
title: 2681 attack Simulator i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305349"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="a8a4a-102">Attack Simulator i Office 365</span><span class="sxs-lookup"><span data-stu-id="a8a4a-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="a8a4a-103">Saknar du attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="a8a4a-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="a8a4a-104">Attack Simulator kräver **office 365 Advanced Threat Protection Plan 2 (ATP-plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="a8a4a-105">Attack Simulator ingår **inte** i Office 365 Advanced Threat Protection Plan 1 (ATP-plan 1), Office 365 Enterprise E3 eller Office 365 Business-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="a8a4a-106">Det konto som du använder för att starta simulerade attacker kräver global administratör eller säkerhets administratörsbehörighet och multifaktorautentisering (MFA).</span><span class="sxs-lookup"><span data-stu-id="a8a4a-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="a8a4a-107">Mer information om krav för attack Simulator finns i [det här avsnittet](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="a8a4a-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="a8a4a-108">Viktiga saker att veta om **brute force lösenord** attack simuleringar:</span><span class="sxs-lookup"><span data-stu-id="a8a4a-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="a8a4a-109">Om målkontot har MFA aktiverat och lösenordet gissades korrekt, visas kontot inte som komprometterad (den andra autentiseringsfaktorn blir ofullständig).</span><span class="sxs-lookup"><span data-stu-id="a8a4a-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="a8a4a-110">Lösenordsfilen får inte vara större än 10 MB.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="a8a4a-111">Använd ett lösenord per rad och inkludera en tom rad (vagnretur) efter det sista lösenordet i listan.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="a8a4a-112">Viktiga saker att veta om **spjut phishing** bifoga simuleringar:</span><span class="sxs-lookup"><span data-stu-id="a8a4a-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="a8a4a-113">Du kan inte ange ett anpassat värde för URL för **phishing-inloggningserver**.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="a8a4a-114">Om en mottagare använder den [Aktivera rapportmeddelande tillägget](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) för att rapportera meddelandet som nätfiske, kanske du inte får aviseringar för meddelandet (eftersom detta är en simulerad attack).</span><span class="sxs-lookup"><span data-stu-id="a8a4a-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="a8a4a-115">Rapporter: när den simulerade attacken är klar kan du klicka på **attack Detaljer** för att se rapporten.</span><span class="sxs-lookup"><span data-stu-id="a8a4a-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="a8a4a-116">Detaljerade instruktioner och nya funktioner i attack Simulator finns i [attack Simulator i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="a8a4a-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
