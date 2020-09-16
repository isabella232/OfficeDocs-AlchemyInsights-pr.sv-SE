---
title: Felsöka certifikat distributionen för klientautentisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659004"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="0ee58-102">Felsöka certifikat distributionen för klientautentisering</span><span class="sxs-lookup"><span data-stu-id="0ee58-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="0ee58-103">Intune NDES-och SCEP-och PKCS/PFX-klient certifikat profiler används ofta tillsammans med andra profil typer, till exempel WiFi, VPN och e-post för att tillåta användare att autentiseras för företagets resurser.</span><span class="sxs-lookup"><span data-stu-id="0ee58-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="0ee58-104">När dessa profil typer är länkade till en profil för klient certifikat beror på distributionen av profilen.</span><span class="sxs-lookup"><span data-stu-id="0ee58-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="0ee58-105">Installation av första infrastruktur och konfiguration av klient certifikat profilen kräver ofta fel sökning.</span><span class="sxs-lookup"><span data-stu-id="0ee58-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="0ee58-106">En steg-för-steg-guide till lyckad konfiguration av NDES Connector och fel söknings råd för att isolera problem med certifikat distribution finns i:</span><span class="sxs-lookup"><span data-stu-id="0ee58-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="0ee58-107">Konfigurera infrastrukturen för att stödja SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="0ee58-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="0ee58-108">Översikt för fel sökning av SCEP-certifikat profiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0ee58-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="0ee58-109">Använd de refererade PowerShell-skripten för att verifiera din konfiguration.</span><span class="sxs-lookup"><span data-stu-id="0ee58-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="0ee58-110">Mer information finns i artikeln om [verifiering av Intune Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="0ee58-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="0ee58-111">**Andra vanliga problem**</span><span class="sxs-lookup"><span data-stu-id="0ee58-111">**Other common issues**</span></span>

<span data-ttu-id="0ee58-112">**När jag försöker installera Intune-certifikattjänsterna på NDES Connector-servern får jag meddelandet "lösen ordet i certifikatbegäran kan inte verifieras. Den kanske redan har använts. Få ett nytt lösen ord att skicka med denna begäran. "**</span><span class="sxs-lookup"><span data-stu-id="0ee58-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="0ee58-113">Det här meddelandet innebär att du måste köra installationen av certifikatanslutningsappen som administratör.</span><span class="sxs-lookup"><span data-stu-id="0ee58-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="0ee58-114">I vissa miljöer måste de servrar där Intune-certifikatet körs använda en proxyserver för att ansluta till Intune och så att certifikat kopplingen måste använda en proxy.</span><span class="sxs-lookup"><span data-stu-id="0ee58-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="0ee58-115">I vissa fall ignorerar NDES Connector de konfigurerade proxyinställningarna och det kan vara nödvändigt att konfigurera proxyinställningarna när de körs i säkerhets kontexten för LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="0ee58-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="0ee58-116">Lösningen är att köra Internet Explorer som SYSTEM och konfigurera en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="0ee58-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="0ee58-117">När du har startat om Intune Connector-tjänsten ansluter NDES Connector till Intune.</span><span class="sxs-lookup"><span data-stu-id="0ee58-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="0ee58-118">**Användar enheter tar inte längre emot SCEP-certifikat från NDES.**</span><span class="sxs-lookup"><span data-stu-id="0ee58-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="0ee58-119">Det är möjligt att certifikatet för klientautentisering som utfärdas till NDES-servern och angavs under installationen av NDES Connector har upphört att gälla eller saknas.</span><span class="sxs-lookup"><span data-stu-id="0ee58-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="0ee58-120">Så här löser du:</span><span class="sxs-lookup"><span data-stu-id="0ee58-120">To resolve:</span></span> 
 
1. <span data-ttu-id="0ee58-121">Avinstallera NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="0ee58-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="0ee58-122">Använd dessa uppgifter för att begära en ny klientautentisering eller Server certifikat:</span><span class="sxs-lookup"><span data-stu-id="0ee58-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="0ee58-123">Ämnes namn: CN = externt FQDN</span><span class="sxs-lookup"><span data-stu-id="0ee58-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="0ee58-124">Alternativa namn för subjekt (båda är obligatoriska): DNS = extern FQDN, DNS = internt FQDN</span><span class="sxs-lookup"><span data-stu-id="0ee58-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="0ee58-125">Installera om NDES Connector med det nya certifikatet.</span><span class="sxs-lookup"><span data-stu-id="0ee58-125">Reinstall the NDES connector with the new certificate.</span></span>