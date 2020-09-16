---
title: 2681 angrepps Simulator i Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759237"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="ab145-102">Angrepps Simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ab145-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="ab145-103">Saknar du angrepps Simulator?</span><span class="sxs-lookup"><span data-stu-id="ab145-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="ab145-104">För angrepps Simulator krävs **office 365 Advanced Threat Protection Plan 2 (ATP-abonnemang 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="ab145-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="ab145-105">Angrepps Simulator ingår **inte** i Office 365 Avancerat skydds abonnemang 1 (ATP-abonnemang 1), Office 365 Enterprise E3 eller något Microsoft 365-program för Business-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="ab145-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="ab145-106">Det konto som du använder för att starta simulerade attacker kräver den globala administratören eller säkerhets administratören och multifaktorautentisering.</span><span class="sxs-lookup"><span data-stu-id="ab145-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="ab145-107">Mer information om krav för attack simulatorn finns i [det här avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ab145-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="ab145-108">Viktiga saker du bör veta om att simulering av **lösen ords attacker är brutet** :</span><span class="sxs-lookup"><span data-stu-id="ab145-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="ab145-109">Om det finns MFA aktiverat för mål kontot och lösen ordet har gissats till är det inte säkert att kontot påverkas (den andra autentiseringsprocessen är ofullständigt).</span><span class="sxs-lookup"><span data-stu-id="ab145-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="ab145-110">Lösen ords filen får inte vara större än 10 MB.</span><span class="sxs-lookup"><span data-stu-id="ab145-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="ab145-111">Använd ett lösen ord per rad och inkludera en tom rad (rad matning) efter det senaste lösen ordet i listan.</span><span class="sxs-lookup"><span data-stu-id="ab145-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="ab145-112">Viktiga saker du bör veta om **Spear nät fiske** :</span><span class="sxs-lookup"><span data-stu-id="ab145-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="ab145-113">Efter design kan du inte ange ett anpassat värde för **URL-adressen till nätfiske-inloggningen**.</span><span class="sxs-lookup"><span data-stu-id="ab145-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="ab145-114">Om en mottagare använder [tillägget aktivera rapport meddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) om du vill rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är ett simulerat angrepp).</span><span class="sxs-lookup"><span data-stu-id="ab145-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="ab145-115">Rapporter: när det simulerade angreppet är slutfört kan du klicka på **angrepps information** för att visa rapporten.</span><span class="sxs-lookup"><span data-stu-id="ab145-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="ab145-116">Detaljerade instruktioner och nya funktioner i angrepps Simulator finns i [angrepps Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ab145-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
