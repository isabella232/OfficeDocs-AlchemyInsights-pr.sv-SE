---
title: Lösa felmeddelanden om olicensierad produkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786867"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="7536e-102">Förslag på hur du löser "Olicensierad produkt"-fel</span><span class="sxs-lookup"><span data-stu-id="7536e-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="7536e-103">Prova följande för att lösa fel om en "Olicensierad produkt":</span><span class="sxs-lookup"><span data-stu-id="7536e-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="7536e-104">Kontrollera om din prenumerationsstatus har upphört att gälla.</span><span class="sxs-lookup"><span data-stu-id="7536e-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="7536e-105">Kontrollera att du har en prenumeration som tillåter klientlicenser, till exempel Microsoft 365-appar för företag eller Business Premium, och kontrollera att användaren har [en tilldelad licens.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="7536e-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="7536e-106">Kontrollera att användaren loggar in på Office med samma konto som licensen har tilldelats.</span><span class="sxs-lookup"><span data-stu-id="7536e-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="7536e-107">Kontrollera sidan [Tjänstens hälsa](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns kända problem med tjänsten.</span><span class="sxs-lookup"><span data-stu-id="7536e-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="7536e-108">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Microsoft 365-apparna åtkomst till Internet.</span><span class="sxs-lookup"><span data-stu-id="7536e-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="7536e-109">Se [URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="7536e-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="7536e-110">Du kan också prova följande felsökningsåtgärder:</span><span class="sxs-lookup"><span data-stu-id="7536e-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="7536e-111">Öppna ett Office-program [och logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="7536e-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="7536e-112">[Ta](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) bort [och tilldela Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) igen och logga [sedan in på Office med](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) det aktuella användarkontot.</span><span class="sxs-lookup"><span data-stu-id="7536e-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="7536e-113">Kör [felsökaren för aktivering.](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="7536e-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="7536e-114">[Återställ Office-aktiveringsstatusen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="7536e-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="7536e-115">[Utföra en onlinereparation av Office.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="7536e-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="7536e-116">Ytterligare lösningar för felsökning finns i:</span><span class="sxs-lookup"><span data-stu-id="7536e-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="7536e-117">Office-felmeddelanden om olicensierad produkt och aktivering</span><span class="sxs-lookup"><span data-stu-id="7536e-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="7536e-118">Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office</span><span class="sxs-lookup"><span data-stu-id="7536e-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)