---
title: Avhjälpa fel om att programmet inte identifierades
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666996"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="12850-102">Avhjälpa fel om att programmet inte identifierades</span><span class="sxs-lookup"><span data-stu-id="12850-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="12850-103">Installationsfelet ”Programmet kunde inte identifieras när installationen hade slutförts” som rapporteras av Intune kan uppstå på alla större operativsystemsplattformar (Windows, iOS och Android).</span><span class="sxs-lookup"><span data-stu-id="12850-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="12850-104">De vanligaste scenarier som genererar felet är:</span><span class="sxs-lookup"><span data-stu-id="12850-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="12850-105">Appen har uppdaterats utanför Intune (via en appbutik från tredje part) efter den första distributionen.</span><span class="sxs-lookup"><span data-stu-id="12850-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="12850-106">Vissa program, till exempel Google Chrome, kan utföra automatiska uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="12850-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="12850-107">En användare har avinstallerat appen efter den första installationen.</span><span class="sxs-lookup"><span data-stu-id="12850-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="12850-108">Om du vill avhjälpa problemet måste du först granska de berörda enheterna för att avgöra vilket scenario som orsakat felet.</span><span class="sxs-lookup"><span data-stu-id="12850-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="12850-109">Om appen har uppdaterats utanför Intune kan programdistributionen ställas in att ignorera programversionen.</span><span class="sxs-lookup"><span data-stu-id="12850-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="12850-110">Om du vill göra det går du till **Appkonfigurering > Appinformation** och ställer in **Ignorera appversion** på **Ja**.</span><span class="sxs-lookup"><span data-stu-id="12850-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="12850-111">När det gäller klienten kan det vara lämpligt att appen distribueras ”efter behov” och att säkerställa att den senaste versionen distribueras.</span><span class="sxs-lookup"><span data-stu-id="12850-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="12850-112">Alternativt kan du på iOS-plattformen använda funktionen för **automatisk uppdatering** som associeras med Apples volyminköpsprogram och som kan konfigureras så att den uppdateras automatiskt till nya appversioner när de blir tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="12850-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="12850-113">Mer information om hur du felsöker problem med appinstallationer finns i [Felsöka problem med appinstallationer](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="12850-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
