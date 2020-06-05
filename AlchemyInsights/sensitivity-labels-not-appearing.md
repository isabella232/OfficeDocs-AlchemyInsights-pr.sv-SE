---
title: Känslighetsetiketter visas inte
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581033"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="67816-102">Känslighetsetiketter visas inte</span><span class="sxs-lookup"><span data-stu-id="67816-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="67816-103">Med känslighetsetiketter kan du klassificera och skydda ditt känsliga innehåll.</span><span class="sxs-lookup"><span data-stu-id="67816-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="67816-104">De kan skapas i Microsoft 365 compliance center, Microsoft 365 security center eller Microsoft 365 security & Compliance Center under Klassificering > känslighetsetiketter.</span><span class="sxs-lookup"><span data-stu-id="67816-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="67816-105">Mer information om den här funktionen finns i [Översikt över känslighetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="67816-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="67816-106">Om du har konfigurerat känslighetsetiketterna men inte visas i Microsoft 365-apparna kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="67816-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="67816-107">Bekräfta att känslighetsetiketten har [publicerats](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) för de användare och grupper som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="67816-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="67816-108">Bekräfta att användaren använder en app som stöder känslighetsetiketter – se [känslighetsetiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="67816-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="67816-109">Om du [migrerar Azure Information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)bör du vara medveten om de överväganden som anges [här](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="67816-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="67816-110">DLP-stöd (Data loss prevention) : För närvarande kan endast kvarhållningsetiketter användas som ett villkor i DLP-principer.</span><span class="sxs-lookup"><span data-stu-id="67816-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="67816-111">Stöd för känslighetsetiketter i en DLP-princip är inte tillgängligt ännu, men vi arbetar på det.</span><span class="sxs-lookup"><span data-stu-id="67816-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="67816-112">När kryptering är aktiverat på en känslighetsetikett kan du välja att antingen:</span><span class="sxs-lookup"><span data-stu-id="67816-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="67816-113">Tilldela behörigheter nu</span><span class="sxs-lookup"><span data-stu-id="67816-113">Assign permissions now</span></span>
    - <span data-ttu-id="67816-114">Låta användare tilldela behörigheter</span><span class="sxs-lookup"><span data-stu-id="67816-114">Let users assign permissions</span></span>


<span data-ttu-id="67816-115">Mer information om möjliga problem finns i [Kända problem med känslighetsetiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="67816-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>