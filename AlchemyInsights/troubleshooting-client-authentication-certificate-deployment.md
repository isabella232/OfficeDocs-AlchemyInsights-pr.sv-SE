---
title: Felsöka distribution av klientautentiseringscertifikat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555808"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="1fbe6-102">Felsöka distribution av klientautentiseringscertifikat</span><span class="sxs-lookup"><span data-stu-id="1fbe6-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="1fbe6-103">Intune NDES/SCEP- och PKCS/PFX-klientcertifikatprofiler används ofta tillsammans med andra profiltyper som Wifi, VPN och e-post så att användare kan autentisera till företagsresurser.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="1fbe6-104">När dessa profiltyper är länkade till en klientcertifikatprofil är beroende av en lyckad distribution av den profilen.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="1fbe6-105">Inledande infrastrukturinstallation och tillhörande konfiguration av klientcertifikatprofilen kräver ofta felsökning.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="1fbe6-106">En steg-för-steg-guide till en lyckad installation av NDES-anslutnings- och felsökningsvägledningen för att isolera problem med certifikatdistributionen finns i:</span><span class="sxs-lookup"><span data-stu-id="1fbe6-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="1fbe6-107">Konfigurera infrastruktur för att stödja SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="1fbe6-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="1fbe6-108">Översikt för felsökning av SCEP-certifikatprofiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1fbe6-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="1fbe6-109">Använd de refererade powershellskripten för att verifiera konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="1fbe6-110">Mer information finns i [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="1fbe6-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="1fbe6-111">**Andra vanliga frågor**</span><span class="sxs-lookup"><span data-stu-id="1fbe6-111">**Other common issues**</span></span>

<span data-ttu-id="1fbe6-112">**När jag försöker installera Intune-certifikatanslutningen på NDES-anslutningsservern får jag meddelandet "Lösenordet i certifikatbegäran kan inte verifieras. Det kan redan ha använts. Skaffa ett nytt lösenord att skicka med den här begäran."**</span><span class="sxs-lookup"><span data-stu-id="1fbe6-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="1fbe6-113">Det här meddelandet innebär att du måste köra installationen av certifikatanslutningen som administratör.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="1fbe6-114">I vissa miljöer måste servrarna där Intune-certifikatet körs använda en proxyserver för att ansluta till Intune, och därför måste certifikatanslutningen använda en proxy.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="1fbe6-115">I vissa fall ignorerar NDES Connector de konfigurerade proxyinställningarna och det kan vara nödvändigt att konfigurera proxyinställningarna när du kör i säkerhetskontexten för LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="1fbe6-116">Lösningen är att köra Internet Explorer som SYSTEM och konfigurera en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="1fbe6-117">Efter en omstart av Intune Connector Service ansluter NDES Connector till Intune.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="1fbe6-118">**Användarenheter får inte längre SCEP-certifikat från NDES.**</span><span class="sxs-lookup"><span data-stu-id="1fbe6-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="1fbe6-119">Det är möjligt att klientautentiseringscertifikatet som utfärdats till NDES-servern och som angavs under installationen av NDES-anslutning, har upphört att gälla eller saknas.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="1fbe6-120">Så här löser du:</span><span class="sxs-lookup"><span data-stu-id="1fbe6-120">To resolve:</span></span> 
 
1. <span data-ttu-id="1fbe6-121">Avinstallera NDES-kontakten.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="1fbe6-122">Använd den här informationen för att begära ett nytt certifikat för klientautentisering eller serverautentisering:</span><span class="sxs-lookup"><span data-stu-id="1fbe6-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="1fbe6-123">Ämnesnamn: CN=extern fqdn</span><span class="sxs-lookup"><span data-stu-id="1fbe6-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="1fbe6-124">Ämnesalternativnamn (båda krävs): DNS=extern fqdn, DNS=intern fqdn</span><span class="sxs-lookup"><span data-stu-id="1fbe6-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="1fbe6-125">Installera om NDES-anslutningen med det nya certifikatet.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-125">Reinstall the NDES connector with the new certificate.</span></span>