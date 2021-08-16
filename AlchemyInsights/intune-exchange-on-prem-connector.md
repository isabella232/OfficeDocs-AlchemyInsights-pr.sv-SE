---
title: Intune Exchange lokal koppling
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013982"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokal koppling

Information om hur du inställningar för anslutningen mellan Intune och Exchange som ligger lokalt finns i följande dokumentation:

[Konfigurera den lokala Intune-anslutningen Exchange i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Vanliga frågor och svar:**

F: Jag ser ett felmeddelande, till exempel "Exchange-kopplingsversionen stöds inte" när jag försöker konfigurera Exchange anslutaren. Vad kan vara orsaken?

S: Det konto som du använder är licensierat på rätt sätt – det måste ha en aktiv Intune-licens

F: Går det att ha flera Exchange kopplingar?

S: Du kan bara konfigurera en enda Exchange per Intune-klientorganisation per Exchange organisation. Anslutningen kan bara installeras på en server i en organisation med flera servrar för Exchange.

Du kan inte heller ha kopplingar konfigurerade för Exchange lokala och lokala Exchange Online konfigureras i samma klientorganisation.

F: Kan kopplingen använda en CAS-matris som koppling till Exchange?

S: Det går inte att ange en CAS-matris i kopplingskonfigurationen. Endast en enskild server bör anges och ska vara hårdkodad i anslutningskonfigurationsfilen som finns i

program data\microsoft\microsoft Intune lokalt Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Leta upp följande post ```<ExchangeWebServiceURL />``` och ersätt URL-adressen med Exchange-servern.

**Exempel:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Se följande dokumentation för ytterligare felsökning: Felsöka den lokala [Intune-Exchange anslutningen](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivera utförlig loggning för Exchange anslutningen**

1. Öppna konfigurationsfilen Exchange kopplingsspårning för redigering.  
Filen finns i : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exempel:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Leta reda på TraceSourceLine med följande nyckel: OnPremisesExchangeConnectorService  
  
3. Ändra SourceLevel-nodvärdet från Information ActivityTracing (standard) till Utförlig aktivitetsstracing  

**Exempel:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Starta om Microsoft Intune Exchange tjänsten  
5. Fullständig synkronisering i Intune-portalen tills den är klar och ändra sedan tillbaka XML-koden till "Information ActivityTracing" och starta om Microsoft Intune Exchange tjänsten.  
6. Platsen för loggarna är: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`