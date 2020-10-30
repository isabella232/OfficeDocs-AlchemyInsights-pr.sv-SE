---
title: Lokal Connector för Intune Exchange
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808140"
---
# <a name="intune-exchange-on-premise-connector"></a>Lokal Connector för Intune Exchange

Information om hur du konfigurerar kopplingen mellan Intune och Exchange som hanteras lokalt finns i följande dokumentation:

[Konfigurera den lokala Intune-anslutaren i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FRÅGORNA**

F: Jag ser ett fel som "Exchange Connector-versionen stöds inte" när jag försöker konfigurera Exchange-anslutaren. Vad kan vara orsaken till?

A: det konto du använder är licensierat-det måste ha en aktiv Intune-licens

F: är det möjligt att ha flera Exchange-kopplingar?

A: du kan bara konfigurera en Exchange-anslutning per Intune-klient per Exchange-organisation. Anslutningen kan bara installeras på en server i en Exchange-organisation med flera servrar.

Du kan inte heller ha anslutningar konfigurerade för både Exchange lokalt och Exchange Online konfigurerat på samma klient organisation.

F: kan kopplingen använda en CAS-matris som anslutning till Exchange?

A: att ange en CAS-matris är inte en konfiguration som stöds i Connector. Det går bara att ange en enda server och det bör vara hårdkodade i anslutnings konfigurations filen som finns i

program data\microsoft\microsoft Intune on Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Leta upp följande post ```<ExchangeWebServiceURL />``` och ersätt URL-adressen med Exchange-servern.

**Exempel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Se följande dokumentation för ytterligare fel sökning: [Felsöka Intune lokala Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivera utförlig loggning för Exchange-anslutaren**

1. Öppna konfigurations filen för Exchange Connector-spårning för redigering.  
Filen finns på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exempel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Leta reda på TraceSourceLine med följande nycklar: OnPremisesExchangeConnectorService  
  
3. Ändra värdet för SourceLevel från informationen ActivityTracing (standard) till verbose-ActivityTracing  

**Exempel**
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
4. Starta om Microsoft Intune Exchange Service  
5. Fullständig synkronisering i Intune-portalen tills den avslut ATS och ändra sedan XML-tillbaka till "informations ActivityTracing" och starta om Microsoft Intune Exchange-tjänsten.  
6. Plats för loggar är: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`