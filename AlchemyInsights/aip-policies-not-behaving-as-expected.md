---
title: 'AIP: Principer fungerar inte som förväntat'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821645"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="f661f-102">AIP: Principer fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="f661f-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="f661f-103">Azure Information Protection: Principer fungerar inte som förväntat. Se följande för rekommenderade riktlinjer för olika principproblem:</span><span class="sxs-lookup"><span data-stu-id="f661f-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="f661f-104">Om du har problem med visuella markeringar kan du läsa [När visuella markeringar används](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="f661f-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f661f-105">Om du har problem med automatisk märkning kan du läsa Konfigurera villkor för automatisk och rekommenderad klassificering för [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och Vilka typer av känslig information letar [efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f661f-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="f661f-106">Om du har problem med inbyggt/Pfilskydd kan du läsa File [API-konfiguration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="f661f-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="f661f-107">Kontrollera om du använder omfattningsprinciper som inte är korrekt konfigurerade: Konfigurera Azure Information Protection-principen för specifika användare med hjälp av [omfattande principer.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="f661f-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="f661f-108">Om automatisk märkning inte fungerar för Outlook när du bifogar ett etiketterat dokument kontrollerar du att DRMEncryptProperty inte har definierats enligt beskrivningen här: IRM-registerinställningar för [säkerhet.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="f661f-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="f661f-109">Om du fortfarande har problem samlar du in Azure Information Protection-klientloggar och bifogar de exporterade loggarna i det här ärendeet.</span><span class="sxs-lookup"><span data-stu-id="f661f-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="f661f-110">Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.</span><span class="sxs-lookup"><span data-stu-id="f661f-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f661f-111">Klicka **på Skydda/känslighet**  >  **Hjälp och feedback.**</span><span class="sxs-lookup"><span data-stu-id="f661f-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f661f-112">Klicka **på Exportera loggar**.</span><span class="sxs-lookup"><span data-stu-id="f661f-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f661f-113">Spara loggarna till ditt val av plats och bifoga dem till denna tjänstbegäran.</span><span class="sxs-lookup"><span data-stu-id="f661f-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f661f-114">Fler resurser:</span><span class="sxs-lookup"><span data-stu-id="f661f-114">Additional resources:</span></span>

- [<span data-ttu-id="f661f-115">Konfigurera en etikett för visuella markeringar för Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f661f-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f661f-116">Granska dokumentationen för Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f661f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f661f-117">Använda känslighetsetiketter i Microsoft 365-appar</span><span class="sxs-lookup"><span data-stu-id="f661f-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

