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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Felsöka certifikat distributionen för klientautentisering

Intune NDES-och SCEP-och PKCS/PFX-klient certifikat profiler används ofta tillsammans med andra profil typer, till exempel WiFi, VPN och e-post för att tillåta användare att autentiseras för företagets resurser. När dessa profil typer är länkade till en profil för klient certifikat beror på distributionen av profilen.

Installation av första infrastruktur och konfiguration av klient certifikat profilen kräver ofta fel sökning. En steg-för-steg-guide till lyckad konfiguration av NDES Connector och fel söknings råd för att isolera problem med certifikat distribution finns i: 

- [Konfigurera infrastrukturen för att stödja SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Översikt för fel sökning av SCEP-certifikat profiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Använd de refererade PowerShell-skripten för att verifiera din konfiguration. Mer information finns i artikeln om [verifiering av Intune Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andra vanliga problem**

**När jag försöker installera Intune-certifikattjänsterna på NDES Connector-servern får jag meddelandet "lösen ordet i certifikatbegäran kan inte verifieras. Den kanske redan har använts. Få ett nytt lösen ord att skicka med denna begäran. "**  

Det här meddelandet innebär att du måste köra installationen av certifikatanslutningsappen som administratör.

I vissa miljöer måste de servrar där Intune-certifikatet körs använda en proxyserver för att ansluta till Intune och så att certifikat kopplingen måste använda en proxy. I vissa fall ignorerar NDES Connector de konfigurerade proxyinställningarna och det kan vara nödvändigt att konfigurera proxyinställningarna när de körs i säkerhets kontexten för LocalSystem. 
 
Lösningen är att köra Internet Explorer som SYSTEM och konfigurera en proxy i IE. När du har startat om Intune Connector-tjänsten ansluter NDES Connector till Intune.

**Användar enheter tar inte längre emot SCEP-certifikat från NDES.**

Det är möjligt att certifikatet för klientautentisering som utfärdas till NDES-servern och angavs under installationen av NDES Connector har upphört att gälla eller saknas. Så här löser du: 
 
1. Avinstallera NDES Connector.  
2. Använd dessa uppgifter för att begära en ny klientautentisering eller Server certifikat: 
 
    - Ämnes namn: CN = externt FQDN  
    - Alternativa namn för subjekt (båda är obligatoriska): DNS = extern FQDN, DNS = internt FQDN 
 
3. Installera om NDES Connector med det nya certifikatet.