---
title: Det gick inte att aktivera Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812590"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="8e473-102">Det gick inte att aktivera Office</span><span class="sxs-lookup"><span data-stu-id="8e473-102">Unable to activate Office</span></span>

- <span data-ttu-id="8e473-103">Kontrollera om prenumerationen har gått ut.</span><span class="sxs-lookup"><span data-stu-id="8e473-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="8e473-104">Kontrollera att du har en prenumeration som tillåter klientlicenser som exempelvis Office 365 Business eller Business Premium, samt att [användaren har en licens tilldelad](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8e473-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="8e473-105">Kontrollera att användaren loggar in i Office med samma konto som tilldelats licensen.</span><span class="sxs-lookup"><span data-stu-id="8e473-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="8e473-106">Gå till [sidan för tjänststatus i Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.</span><span class="sxs-lookup"><span data-stu-id="8e473-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="8e473-107">Kontrollera brandväggen, antivirusprogram och proxyinställningarna för att kontrollera att de inte blockerar Microsoft 365-applikationers åtkomst till internet.</span><span class="sxs-lookup"><span data-stu-id="8e473-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="8e473-108">Gå till [URL-adresser och IP-adressintervall för Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-adresser och IP-adressintervall för Office 365").</span><span class="sxs-lookup"><span data-stu-id="8e473-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="8e473-109">**Tips** På Windows-datorer kan vi diagnostisera och automatiskt korrigera flera vanliga inloggningsproblem för Office åt dig.</span><span class="sxs-lookup"><span data-stu-id="8e473-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8e473-110">Ladda ned och kör **[Support- och återställningsassistenten](https://aka.ms/SaRA-OfficeSignInScenario)** om du vill använda vårt automatiska verktyg.</span><span class="sxs-lookup"><span data-stu-id="8e473-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8e473-111">Använd följande åtgärder för felsökning:</span><span class="sxs-lookup"><span data-stu-id="8e473-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="8e473-112">Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="8e473-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="8e473-113">[Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) och [omtilldela](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen och [logga in i Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det påverkade användarkontot.</span><span class="sxs-lookup"><span data-stu-id="8e473-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="8e473-114">Kör [Aktiveringsfelsökaren](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="8e473-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="8e473-115">Återställ Office-aktiveringsstatus</span><span class="sxs-lookup"><span data-stu-id="8e473-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Återställ Office-aktiveringsstatus")
- [<span data-ttu-id="8e473-116">Kör en onlinereparation av Office</span><span class="sxs-lookup"><span data-stu-id="8e473-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="8e473-117">Ytterligare lösningar för felsökning finns i:</span><span class="sxs-lookup"><span data-stu-id="8e473-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="8e473-118">Office-felmeddelanden om olicensierad produkt och aktivering</span><span class="sxs-lookup"><span data-stu-id="8e473-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="8e473-119">Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office</span><span class="sxs-lookup"><span data-stu-id="8e473-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)