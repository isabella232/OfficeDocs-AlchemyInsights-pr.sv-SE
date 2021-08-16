---
title: Felsöka distribution av certifikat för klientautentisering
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020822"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Felsöka distribution av certifikat för klientautentisering

Profiler för Intune NDES/SITI och PKCS/PFX-klientcertifikat används ofta tillsammans med andra profiltyper, till exempel Wifi, VPN och e-post, så att användarna kan autentisera sig för företagets resurser. När profiltyperna är länkade till en klientcertifikatprofil är beroende av en lyckad distribution av profilen.

Inledande infrastrukturkonfiguration och associerad konfiguration av profilen för klientcertifikat kräver ofta felsökning. Stegvisa instruktioner för hur du lyckas konfigurera NDES-anslutningen och felsökningsvägledning för att identifiera problem med certifikatdistribution finns i: 

- [Konfigurera infrastrukturen som stöder SITI med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Översikt för felsökning av S FLERA-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Använd powershell-skripten som det refereras till för att verifiera konfigurationen. Mer information finns i [Verifieringsskript för Intune-certifikatkoppling.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Andra vanliga problem**

**När jag försöker installera Intune-certifikatkopplingen på NDES-anslutningsservern visas ett meddelande om att lösenordet i certifikatbegäran inte kan verifieras. Den kan redan ha använts. Skaffa ett nytt lösenord för att skicka in med denna begäran."**  

Det här meddelandet innebär att du måste köra installationen av certifikatkopplingen som administratör.

I vissa miljöer måste servrarna där Intune-certifikatet körs använda en proxyserver för att ansluta till Intune, så certifikatkopplingen måste använda en proxy. I vissa fall ignorerar NDES-kopplingen de konfigurerade proxyinställningarna och det kan vara nödvändigt att konfigurera proxyinställningarna medan de körs i säkerhetssammanhanget för LocalSystem. 
 
Lösningen är att köra Internet Explorer som SYSTEM och konfigurera en proxy i IE. Efter en omstart av Intune-kopplingstjänsten ansluter NDES-kopplingen till Intune.

**Användarenheter får inte längre S ÄR-certifikat från NDES.**

Det är möjligt att klientautentiseringscertifikatet som utfärdats till NDES-servern och angetts under installationen av NDES-anslutningen har upphört att gälla eller saknas. Så här löser du det: 
 
1. Avinstallera NDES-kopplingen.  
2. Använd den här informationen för att begära en ny klientautentisering eller ett nytt serverautentiseringscertifikat: 
 
    - Ämnesnamn: CN=extern fqdn  
    - Alternativt ämnesnamn (båda är obligatoriska): DNS=extern fqdn, DNS=intern fqdn 
 
3. Installera om NDES-anslutningen med det nya certifikatet.