---
title: Känslighets etiketter visas inte
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801202"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="8ad35-102">Känslighets etiketter visas inte</span><span class="sxs-lookup"><span data-stu-id="8ad35-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="8ad35-103">Med känslighets etiketter kan du klassificera och skydda känsligt innehåll.</span><span class="sxs-lookup"><span data-stu-id="8ad35-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="8ad35-104">De kan skapas i Microsoft 365 Compliance Center, Microsoft 365 säkerhets Center eller Microsoft 365 Security & Support Center under klassificerings > känslighets etiketter.</span><span class="sxs-lookup"><span data-stu-id="8ad35-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="8ad35-105">Mer information om den här funktionen finns i [Översikt över känslighets etiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="8ad35-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="8ad35-106">Om du har konfigurerat dina känslighets etiketter men inte visas i Microsoft 365-apparna kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="8ad35-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="8ad35-107">Kontrol lera att känslighets etiketten har [publicerats](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) till de användare och grupper som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="8ad35-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="8ad35-108">Bekräfta att användaren använder ett program som stöder känslighets etiketter – se [känslighets etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="8ad35-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="8ad35-109">Om du [migrerar etiketter för Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)bör du tänka på de överväganden som visas [här](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="8ad35-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="8ad35-110">Stöd för data förlust skydd (DLP): just nu kan endast bevarande etiketter användas som villkor i DLP-principer.</span><span class="sxs-lookup"><span data-stu-id="8ad35-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="8ad35-111">Stöd för känslighets etiketter i en DLP-princip är ännu inte tillgängligt, men vi jobbar på det.</span><span class="sxs-lookup"><span data-stu-id="8ad35-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="8ad35-112">När kryptering är aktiverat för en känslighets etikett kan du välja mellan:</span><span class="sxs-lookup"><span data-stu-id="8ad35-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="8ad35-113">Tilldela behörigheter nu</span><span class="sxs-lookup"><span data-stu-id="8ad35-113">Assign permissions now</span></span>
    - <span data-ttu-id="8ad35-114">Låta användare tilldela behörigheter</span><span class="sxs-lookup"><span data-stu-id="8ad35-114">Let users assign permissions</span></span>


<span data-ttu-id="8ad35-115">Mer information om möjliga problem finns i [kända problem med känslighets etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="8ad35-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>