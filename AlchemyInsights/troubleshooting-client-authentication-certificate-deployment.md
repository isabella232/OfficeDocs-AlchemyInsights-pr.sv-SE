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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Felsöka distribution av klientautentiseringscertifikat

Intune NDES/SCEP- och PKCS/PFX-klientcertifikatprofiler används ofta tillsammans med andra profiltyper som Wifi, VPN och e-post så att användare kan autentisera till företagsresurser. När dessa profiltyper är länkade till en klientcertifikatprofil är beroende av en lyckad distribution av den profilen.

Inledande infrastrukturinstallation och tillhörande konfiguration av klientcertifikatprofilen kräver ofta felsökning. En steg-för-steg-guide till en lyckad installation av NDES-anslutnings- och felsökningsvägledningen för att isolera problem med certifikatdistributionen finns i: 

- [Konfigurera infrastruktur för att stödja SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Översikt för felsökning av SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Använd de refererade powershellskripten för att verifiera konfigurationen. Mer information finns i [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andra vanliga frågor**

**När jag försöker installera Intune-certifikatanslutningen på NDES-anslutningsservern får jag meddelandet "Lösenordet i certifikatbegäran kan inte verifieras. Det kan redan ha använts. Skaffa ett nytt lösenord att skicka med den här begäran."**  

Det här meddelandet innebär att du måste köra installationen av certifikatanslutningen som administratör.

I vissa miljöer måste servrarna där Intune-certifikatet körs använda en proxyserver för att ansluta till Intune, och därför måste certifikatanslutningen använda en proxy. I vissa fall ignorerar NDES Connector de konfigurerade proxyinställningarna och det kan vara nödvändigt att konfigurera proxyinställningarna när du kör i säkerhetskontexten för LocalSystem. 
 
Lösningen är att köra Internet Explorer som SYSTEM och konfigurera en proxy i IE. Efter en omstart av Intune Connector Service ansluter NDES Connector till Intune.

**Användarenheter får inte längre SCEP-certifikat från NDES.**

Det är möjligt att klientautentiseringscertifikatet som utfärdats till NDES-servern och som angavs under installationen av NDES-anslutning, har upphört att gälla eller saknas. Så här löser du: 
 
1. Avinstallera NDES-kontakten.  
2. Använd den här informationen för att begära ett nytt certifikat för klientautentisering eller serverautentisering: 
 
    - Ämnesnamn: CN=extern fqdn  
    - Ämnesalternativnamn (båda krävs): DNS=extern fqdn, DNS=intern fqdn 
 
3. Installera om NDES-anslutningen med det nya certifikatet.