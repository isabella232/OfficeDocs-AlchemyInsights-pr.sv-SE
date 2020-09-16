---
title: 'AIP: principer fungerar inte som förväntat'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663207"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="608bd-102">AIP: principer fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="608bd-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="608bd-103">Azure information Protection: principer fungerar inte som förväntat, se nedan för rekommenderade rikt linjer för olika princip problem:</span><span class="sxs-lookup"><span data-stu-id="608bd-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="608bd-104">Om du har problem med de visuella märkningarna kan du gå igenom [när de visuella märkningarna tillämpas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="608bd-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="608bd-105">Om du har problem med automatiska etiketter kan du läsa om [hur du konfigurerar villkoren för automatisk och Rekommenderad klassificering för Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och [vilken känslig information som kan](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)hämtas.</span><span class="sxs-lookup"><span data-stu-id="608bd-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="608bd-106">Om du har problem med inbyggt/pfile-skydd kan du läsa igenom [konfigurationen för fil-API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="608bd-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="608bd-107">Kontrol lera om du använder begränsade principer som inte har kon figurer ATS korrekt: [Konfigurera Azure information Protection policy för specifika användare med hjälp av begränsade principer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="608bd-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="608bd-108">Om automatisk etikett inte fungerar för Outlook när du bifogar ett dokument med etiketter kontrollerar du att DRMEncryptProperty inte har definierats enligt beskrivningen här: [IRM-registerpostens inställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="608bd-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="608bd-109">Om du fortfarande har problem kan du samla in Azure information Protection client-loggar och bifoga de exporterade loggarna till den här biljetten.</span><span class="sxs-lookup"><span data-stu-id="608bd-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="608bd-110">Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.</span><span class="sxs-lookup"><span data-stu-id="608bd-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="608bd-111">Klicka på **skydda/känslighets**  >  **Hjälp och feedback**.</span><span class="sxs-lookup"><span data-stu-id="608bd-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="608bd-112">Klicka på **Exportera loggar**.</span><span class="sxs-lookup"><span data-stu-id="608bd-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="608bd-113">Spara loggarna på valfri plats och bifoga dem till den här tjänst förfrågan.</span><span class="sxs-lookup"><span data-stu-id="608bd-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="608bd-114">Fler resurser:</span><span class="sxs-lookup"><span data-stu-id="608bd-114">Additional resources:</span></span>

- [<span data-ttu-id="608bd-115">Konfigurera en etikett för visuell märkning för Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="608bd-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="608bd-116">Granska dokumentationen för Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="608bd-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="608bd-117">Använda känslighets etiketter i Microsoft 365-appar</span><span class="sxs-lookup"><span data-stu-id="608bd-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

