---
title: Avancerade autentiseringsbegrepp som är tillämpliga i Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398603"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="9e668-102">Avancerade autentiseringsbegrepp som är tillämpliga i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9e668-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="9e668-103">Här följer de avancerade autentiseringsbegreppen som gäller för Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="9e668-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="9e668-104">**Proaktiv autentisering**</span><span class="sxs-lookup"><span data-stu-id="9e668-104">**Proactive Authentication**</span></span>

<span data-ttu-id="9e668-105">När du aktiverar [principen ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) försöker Microsoft Edge proaktivt autentisera inloggade användare via Microsoft-tjänster.</span><span class="sxs-lookup"><span data-stu-id="9e668-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="9e668-106">Med jämna mellanrum används en onlinetjänst för att söka efter ett uppdaterat manifest som innehåller konfiguration som reglerar proaktiv autentisering.</span><span class="sxs-lookup"><span data-stu-id="9e668-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="9e668-107">Fördelar: Proaktiv autentisering möjliggör autentisering till nyckeltjänster, till exempel sidan Ny flik i Office.</span><span class="sxs-lookup"><span data-stu-id="9e668-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="9e668-108">Om Bing används som sökmotor förbättrar proaktiv autentisering prestandan i adressfältet och hjälper till att generera sökresultat som är anpassade efter behoven i ditt företag.</span><span class="sxs-lookup"><span data-stu-id="9e668-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="9e668-109">**Windows Hello CredUI för NTLM-autentisering**</span><span class="sxs-lookup"><span data-stu-id="9e668-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="9e668-110">Om enkel inloggning (SSO) inte är tillgänglig när en webbplats försöker logga in på användaren via NTLM- eller förhandlasmekanismen gör den här funktionen att användaren kan dela operativsystemets autentiseringsuppgifter med webbplatsen och uppfylla autentiseringsutmaningen med hjälp av windows Hello-gränssnittet i Cred.</span><span class="sxs-lookup"><span data-stu-id="9e668-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="9e668-111">Det här inloggningsflödet visas bara i Windows 10 och bara för användare som inte får SSO under en NTLM- eller en förhandlans utmaning.</span><span class="sxs-lookup"><span data-stu-id="9e668-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="9e668-112">**Använd sparade lösenord för att logga in automatiskt**</span><span class="sxs-lookup"><span data-stu-id="9e668-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="9e668-113">Användare som sparar lösenord i Microsoft Edge kan aktivera automatisk inloggning på webbplatser där de har sparat autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="9e668-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="9e668-114">Användare kan aktivera eller inaktivera den här funktionen i edge://settings/passwords, och du kan konfigurera den i [lösenordshanterarens](https://go.microsoft.com/fwlink/?linkid=2134622) principer.</span><span class="sxs-lookup"><span data-stu-id="9e668-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
