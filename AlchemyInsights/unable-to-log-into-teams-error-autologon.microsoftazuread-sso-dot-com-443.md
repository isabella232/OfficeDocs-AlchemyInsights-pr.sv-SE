---
title: Det går inte att logga in på Teams på grund av fel autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932287"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="9c5ff-102">Det går inte att logga in på Teams på grund av fel autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="9c5ff-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="9c5ff-103">Om sömlös SSO är aktiverad som O365-autentisering kan URL-adressen "autologon.microsoftazuread-sso.com" behöva läggas till i intranätplatser.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="9c5ff-104">Om den redan har lagts till på betrodda platser och sömlös SSO används ska den tas bort från betrodda platser.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="9c5ff-105">Läs [Checklista för felsökning i sömlös SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="9c5ff-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="9c5ff-106">Följ dessa steg om du vill lägga till en URL-adress i listan över intranät-webbplatser:</span><span class="sxs-lookup"><span data-stu-id="9c5ff-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="9c5ff-107">Öppna Internet Explorer genom att klicka på knappen **Start**.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="9c5ff-108">I sökrutan skriver du Internet Explorer och klickar sedan på **Internet Explorer**i resultatlistan.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="9c5ff-109">Klicka på **Verktyg**och klicka sedan på **Internetalternativ**.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="9c5ff-110">Klicka på fliken **Säkerhet**.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="9c5ff-111">Klicka nu på **Lokala intranät-webbplatser** och klicka sedan på knappen **Webbplatser** och sedan knappen **Avancerat**.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="9c5ff-112">Ange webbplatsens URL och klicka på **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="9c5ff-113">Klicka på **Stäng** när du är klar.</span><span class="sxs-lookup"><span data-stu-id="9c5ff-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="9c5ff-114">Mer information finns i [Dokumentation för distribution av sömlös SSO för O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inkluderar principbaserad process för att lägga till en URL-adress till intranät-webbplatser i steg 3).</span><span class="sxs-lookup"><span data-stu-id="9c5ff-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
