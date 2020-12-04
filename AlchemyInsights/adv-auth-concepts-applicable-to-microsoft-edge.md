---
title: Avancerade autentiseringsmetoder för Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573778"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="cc998-102">Avancerade autentiseringsmetoder för Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cc998-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="cc998-103">Nedan följer de avancerade autentiseringsmetoderna som gäller för Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="cc998-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="cc998-104">**Proaktiv auktorisering**</span><span class="sxs-lookup"><span data-stu-id="cc998-104">**Proactive Authentication**</span></span>

<span data-ttu-id="cc998-105">När du aktiverar [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -principen försöker Microsoft Edge proaktivt autentisera inloggade användare via Microsoft-tjänster.</span><span class="sxs-lookup"><span data-stu-id="cc998-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="cc998-106">Med jämna mellanrum används en online tjänst för att söka efter ett uppdaterat manifest som innehåller konfigurationen som styr proaktiv-förauktoriseringen.</span><span class="sxs-lookup"><span data-stu-id="cc998-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="cc998-107">Fördelar: proaktivt-verifikation möjliggör till gång till viktiga tjänster, till exempel sidan ny flik i Office.</span><span class="sxs-lookup"><span data-stu-id="cc998-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="cc998-108">Om Bing används som sökmotor förbättrar dessutom adress fältets prestanda och gör att Sök resultaten anpassas efter företagets behov?.</span><span class="sxs-lookup"><span data-stu-id="cc998-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="cc998-109">**Windows Hello-CredUI för NTLM-verifikation**</span><span class="sxs-lookup"><span data-stu-id="cc998-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="cc998-110">Om enkel inloggning (SSO) inte är tillgängligt när en webbplats försöker logga in användaren via NTLM eller Negotiate-mekanismen tillåter den här funktionen att användaren delar autentiseringsuppgifterna för operativ systemet med webbplatsen och för att uppfylla verifierings utmaningen genom att använda Windows Hello-gränssnittet.</span><span class="sxs-lookup"><span data-stu-id="cc998-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="cc998-111">Det här inloggnings flödet visas bara i Windows 10 och endast för användare som inte behöver SSO under ett NTLM-eller Negotiate-anrop.</span><span class="sxs-lookup"><span data-stu-id="cc998-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="cc998-112">**Använda sparade lösen ord för att logga in automatiskt**</span><span class="sxs-lookup"><span data-stu-id="cc998-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="cc998-113">Användare som sparar lösen ord i Microsoft Edge kan aktivera automatisk inloggning på webbplatser där de har sparat sina autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="cc998-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="cc998-114">Användare kan aktivera eller inaktivera den här funktionen i edge://settings/passwords och du kan konfigurera den i principer för [lösen ords hanteraren](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="cc998-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
