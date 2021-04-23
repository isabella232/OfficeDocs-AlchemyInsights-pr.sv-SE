---
title: DLP-principtips fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958720"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="fc8ba-102">Problem med DLP-policytips</span><span class="sxs-lookup"><span data-stu-id="fc8ba-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="fc8ba-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fc8ba-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fc8ba-104">Så här konfigurerar du principtips för DLP-principen i säkerhets- & säkerhets- och efterlevnadscenter i fullständigt tvingande läge:</span><span class="sxs-lookup"><span data-stu-id="fc8ba-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="fc8ba-105">Kontrollera att principtips har **aktiverats** för DLP-regeln.</span><span class="sxs-lookup"><span data-stu-id="fc8ba-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="fc8ba-106">Instruktioner finns i Skicka [e-postaviseringar och visa principtips för DLP-principer.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="fc8ba-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="fc8ba-107">Se till att ditt innehåll matchar det som krävs för att utlösa regeln som beskrivs i [definitionerna för entitet av typen Känslig information.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="fc8ba-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="fc8ba-108">Policytips visas i både OWA och Outlook.</span><span class="sxs-lookup"><span data-stu-id="fc8ba-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="fc8ba-109">Men när du använder Outlook 2013 eller senare visas principtips endast under vissa förhållanden.</span><span class="sxs-lookup"><span data-stu-id="fc8ba-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="fc8ba-110">Listan med specifika villkor finns i Villkor [som stöds för Outlook 2013 eller senare för visning av policytips.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="fc8ba-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="fc8ba-111">Mer information om DLP-principtips finns i [Referens för DLP-principtips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) och [Supportmatris för DLP-principtips.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="fc8ba-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>