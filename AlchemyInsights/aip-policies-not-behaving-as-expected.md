---
title: 'AIP: Principer som inte beter sig som förväntat'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506576"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="fe6de-102">AIP: Principer som inte beter sig som förväntat</span><span class="sxs-lookup"><span data-stu-id="fe6de-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="fe6de-103">Azure Information Protection: Principer som inte fungerar som förväntat, se följande för rekommenderade riktlinjer för olika principproblem:</span><span class="sxs-lookup"><span data-stu-id="fe6de-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="fe6de-104">Om du har problem med visuella markeringar läser du [När visuella markeringar används](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="fe6de-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="fe6de-105">Om du har problem med automatisk märkning läser du Så här konfigurerar du [villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och Vilka känsliga [informationstyper som letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="fe6de-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="fe6de-106">Om du har problem med Native/Pfile-skydd läser du [fil-API-konfigurationen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="fe6de-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="fe6de-107">Kontrollera om du använder begränsade principer som inte är korrekt konfigurerade: [Så här konfigurerar du Azure-informationsskyddsprincipen för specifika användare med hjälp av scoped-principer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="fe6de-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="fe6de-108">Om automatisk märkning inte fungerar för Outlook när du bifogar ett märkt dokument kontrollerar du att DRMEncryptProperty inte definieras som beskrivet här: [IRM-registerinställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="fe6de-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="fe6de-109">Om du fortfarande har problem samlar du in Azure Information Protection-klientloggar och bifogar de exporterade loggarna till den här biljetten.</span><span class="sxs-lookup"><span data-stu-id="fe6de-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="fe6de-110">Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.</span><span class="sxs-lookup"><span data-stu-id="fe6de-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="fe6de-111">Klicka på Hjälp och feedback **om skydd/känslighet**  >  **Help and feedback**.</span><span class="sxs-lookup"><span data-stu-id="fe6de-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="fe6de-112">Klicka på **Exportera loggar**.</span><span class="sxs-lookup"><span data-stu-id="fe6de-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="fe6de-113">Spara loggarna till ditt val av plats och bifoga dem till den här servicebegäran.</span><span class="sxs-lookup"><span data-stu-id="fe6de-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="fe6de-114">Fler resurser:</span><span class="sxs-lookup"><span data-stu-id="fe6de-114">Additional resources:</span></span>

- [<span data-ttu-id="fe6de-115">Konfigurera en etikett för visuella markeringar för Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6de-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="fe6de-116">Granska Azure Information Protection-dokumentation</span><span class="sxs-lookup"><span data-stu-id="fe6de-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="fe6de-117">Använda känslighetsetiketter i Office-appar</span><span class="sxs-lookup"><span data-stu-id="fe6de-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

