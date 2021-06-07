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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798698"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="8772a-102">Det gick inte att aktivera Office</span><span class="sxs-lookup"><span data-stu-id="8772a-102">Unable to activate Office</span></span>

<span data-ttu-id="8772a-103">**Obs!** Om du använder en äldre version av Windows (till exempel Windows 7) ska du kontrollera att TLS 1.2 är aktiverat som standard.</span><span class="sxs-lookup"><span data-stu-id="8772a-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="8772a-104">Mer information finns i Uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.</span><span class="sxs-lookup"><span data-stu-id="8772a-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="8772a-105">Kontrollera om prenumerationen har gått ut.</span><span class="sxs-lookup"><span data-stu-id="8772a-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="8772a-106">Kontrollera att du har en prenumeration som tillåter klientlicenser som exempelvis Office 365 Business eller Business Premium, samt att [användaren har en licens tilldelad](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="8772a-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="8772a-107">Kontrollera att användaren loggar in i Office med samma konto som tilldelats licensen.</span><span class="sxs-lookup"><span data-stu-id="8772a-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="8772a-108">Gå till [sidan för tjänststatus i Office 365](/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.</span><span class="sxs-lookup"><span data-stu-id="8772a-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="8772a-109">Kontrollera brandväggen, antivirusprogram och proxyinställningarna för att kontrollera att de inte blockerar Microsoft 365-applikationers åtkomst till internet.</span><span class="sxs-lookup"><span data-stu-id="8772a-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="8772a-110">Gå till [URL-adresser och IP-adressintervall för Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-adresser och IP-adressintervall för Office 365").</span><span class="sxs-lookup"><span data-stu-id="8772a-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="8772a-111">**Tips** På Windows-datorer kan vi diagnostisera och automatiskt korrigera flera vanliga inloggningsproblem för Office åt dig.</span><span class="sxs-lookup"><span data-stu-id="8772a-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8772a-112">Ladda ned och kör **[Support- och återställningsassistenten](https://aka.ms/SaRA-OfficeSignInScenario)** om du vill använda vårt automatiska verktyg.</span><span class="sxs-lookup"><span data-stu-id="8772a-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8772a-113">Använd följande åtgärder för felsökning:</span><span class="sxs-lookup"><span data-stu-id="8772a-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="8772a-114">Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="8772a-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="8772a-115">[Ta bort](/microsoft-365/admin/manage/remove-licenses-from-users) och [omtilldela](/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen och [logga in i Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det påverkade användarkontot.</span><span class="sxs-lookup"><span data-stu-id="8772a-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="8772a-116">Kör [Aktiveringsfelsökaren](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="8772a-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="8772a-117">Återställ Office-aktiveringsstatus</span><span class="sxs-lookup"><span data-stu-id="8772a-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Återställ Office-aktiveringsstatus")
- [<span data-ttu-id="8772a-118">Kör en onlinereparation av Office</span><span class="sxs-lookup"><span data-stu-id="8772a-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="8772a-119">Ytterligare lösningar för felsökning finns i:</span><span class="sxs-lookup"><span data-stu-id="8772a-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="8772a-120">Office-felmeddelanden om olicensierad produkt och aktivering</span><span class="sxs-lookup"><span data-stu-id="8772a-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="8772a-121">Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office</span><span class="sxs-lookup"><span data-stu-id="8772a-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)