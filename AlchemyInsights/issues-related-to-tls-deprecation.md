---
title: Det går inte att skicka/ta emot e-post till/från Office 365 på grund av inaktiveringen av TLS 1.0 och TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747115"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Det går inte att skicka/ta emot e-post till/från Office 365 på grund av inaktiveringen av TLS 1.0 och TLS 1.1

Enligt bekräftelse från meddelandecentret efter MC229914 började utfasningen av TLS 1.0 och TLS 1.1 att tillämpa för e-postflödesslutpunkter i Exchange Online. Snart accepterar Office 365 inte längre TLS 1.0- och TLS 1.1-e-postanslutningar från externa källor. Exchange Online använder heller aldrig TLS 1.0 eller 1.1 för att skicka utgående e-post. Om du har problem på grund av inaktiveringen av TLS 1.0 eller 1.1 kan något av följande felmeddelanden visas:

- Avsändaren får NDR att studsa tillbaka – '421 4.4.2 Anslutningen har släppts på grund av SocketError'
- Felet i kövisningsprogrammet på den lokala servern som skickar e-post till konstapel 365- '421 4.4.2 Anslutningen har släppts på grund av SocketError'
- Fel i loggen för [Skicka kopplingsprotokoll](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) på servern som skickar e-post till Office 365- TLS-förhandling misslyckades med fel SocketError
- Fel i Skicka eller ta emot anslutningsprotokolllogg - '451 5.7.3 Måste utfärda ett STARTTLS-kommando först'

Om något av ovanstående fel uppstår kontrollerar du att servern som skickar eller tar emot e-post har TLS 1.2 aktiverat genom att kontrollera följande registernycklar:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001**

Om du gör någon ändring i registernycklarna ovan för att aktivera TLS 1.2 startar du om servern för att ändringarna ska börja gälla. Kontrollera också att du har de senaste Windows- och Exchange-uppdateringarna installerade.

Mer information finns i:

- [TLS-vägledning för Exchange Server, del 1: För förbereda för TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-vägledning Del 2: Aktivera TLS 1.2 och Identifiera klienter som inte använder det – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Förstå e-postscenarier om det inte går att komma överens om TLS-versioner med Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
