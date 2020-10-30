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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="fca52-102">Lokal Connector för Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="fca52-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="fca52-103">Information om hur du konfigurerar kopplingen mellan Intune och Exchange som hanteras lokalt finns i följande dokumentation:</span><span class="sxs-lookup"><span data-stu-id="fca52-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="fca52-104">Konfigurera den lokala Intune-anslutaren i Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="fca52-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="fca52-105">**FRÅGORNA**</span><span class="sxs-lookup"><span data-stu-id="fca52-105">**FAQ:**</span></span>

<span data-ttu-id="fca52-106">F: Jag ser ett fel som "Exchange Connector-versionen stöds inte" när jag försöker konfigurera Exchange-anslutaren.</span><span class="sxs-lookup"><span data-stu-id="fca52-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="fca52-107">Vad kan vara orsaken till?</span><span class="sxs-lookup"><span data-stu-id="fca52-107">What could be the cause?</span></span>

<span data-ttu-id="fca52-108">A: det konto du använder är licensierat-det måste ha en aktiv Intune-licens</span><span class="sxs-lookup"><span data-stu-id="fca52-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="fca52-109">F: är det möjligt att ha flera Exchange-kopplingar?</span><span class="sxs-lookup"><span data-stu-id="fca52-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="fca52-110">A: du kan bara konfigurera en Exchange-anslutning per Intune-klient per Exchange-organisation.</span><span class="sxs-lookup"><span data-stu-id="fca52-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="fca52-111">Anslutningen kan bara installeras på en server i en Exchange-organisation med flera servrar.</span><span class="sxs-lookup"><span data-stu-id="fca52-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="fca52-112">Du kan inte heller ha anslutningar konfigurerade för både Exchange lokalt och Exchange Online konfigurerat på samma klient organisation.</span><span class="sxs-lookup"><span data-stu-id="fca52-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="fca52-113">F: kan kopplingen använda en CAS-matris som anslutning till Exchange?</span><span class="sxs-lookup"><span data-stu-id="fca52-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="fca52-114">A: att ange en CAS-matris är inte en konfiguration som stöds i Connector.</span><span class="sxs-lookup"><span data-stu-id="fca52-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="fca52-115">Det går bara att ange en enda server och det bör vara hårdkodade i anslutnings konfigurations filen som finns i</span><span class="sxs-lookup"><span data-stu-id="fca52-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="fca52-116">program data\microsoft\microsoft Intune on Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="fca52-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="fca52-117">Leta upp följande post ```<ExchangeWebServiceURL />``` och ersätt URL-adressen med Exchange-servern.</span><span class="sxs-lookup"><span data-stu-id="fca52-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="fca52-118">**Exempel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="fca52-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="fca52-119">Se följande dokumentation för ytterligare fel sökning: [Felsöka Intune lokala Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="fca52-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="fca52-120">**Aktivera utförlig loggning för Exchange-anslutaren**</span><span class="sxs-lookup"><span data-stu-id="fca52-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="fca52-121">Öppna konfigurations filen för Exchange Connector-spårning för redigering.</span><span class="sxs-lookup"><span data-stu-id="fca52-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="fca52-122">Filen finns på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="fca52-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="fca52-123">**Exempel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="fca52-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="fca52-124">Leta reda på TraceSourceLine med följande nycklar: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="fca52-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="fca52-125">Ändra värdet för SourceLevel från informationen ActivityTracing (standard) till verbose-ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="fca52-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="fca52-126">**Exempel**</span><span class="sxs-lookup"><span data-stu-id="fca52-126">**Example:**</span></span>
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
4. <span data-ttu-id="fca52-127">Starta om Microsoft Intune Exchange Service</span><span class="sxs-lookup"><span data-stu-id="fca52-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="fca52-128">Fullständig synkronisering i Intune-portalen tills den avslut ATS och ändra sedan XML-tillbaka till "informations ActivityTracing" och starta om Microsoft Intune Exchange-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="fca52-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="fca52-129">Plats för loggar är: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="fca52-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>