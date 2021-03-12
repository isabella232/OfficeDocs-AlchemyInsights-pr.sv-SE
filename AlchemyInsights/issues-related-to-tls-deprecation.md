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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="c335a-102">Det går inte att skicka/ta emot e-post till/från Office 365 på grund av inaktiveringen av TLS 1.0 och TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="c335a-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="c335a-103">Enligt bekräftelse från meddelandecentret efter MC229914 började utfasningen av TLS 1.0 och TLS 1.1 att tillämpa för e-postflödesslutpunkter i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c335a-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="c335a-104">Snart accepterar Office 365 inte längre TLS 1.0- och TLS 1.1-e-postanslutningar från externa källor.</span><span class="sxs-lookup"><span data-stu-id="c335a-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="c335a-105">Exchange Online använder heller aldrig TLS 1.0 eller 1.1 för att skicka utgående e-post.</span><span class="sxs-lookup"><span data-stu-id="c335a-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="c335a-106">Om du har problem på grund av inaktiveringen av TLS 1.0 eller 1.1 kan något av följande felmeddelanden visas:</span><span class="sxs-lookup"><span data-stu-id="c335a-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="c335a-107">Avsändaren får NDR att studsa tillbaka – '421 4.4.2 Anslutningen har släppts på grund av SocketError'</span><span class="sxs-lookup"><span data-stu-id="c335a-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="c335a-108">Felet i kövisningsprogrammet på den lokala servern som skickar e-post till konstapel 365- '421 4.4.2 Anslutningen har släppts på grund av SocketError'</span><span class="sxs-lookup"><span data-stu-id="c335a-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="c335a-109">Fel i loggen för [Skicka kopplingsprotokoll](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) på servern som skickar e-post till Office 365- TLS-förhandling misslyckades med fel SocketError</span><span class="sxs-lookup"><span data-stu-id="c335a-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="c335a-110">Fel i Skicka eller ta emot anslutningsprotokolllogg - '451 5.7.3 Måste utfärda ett STARTTLS-kommando först'</span><span class="sxs-lookup"><span data-stu-id="c335a-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="c335a-111">Om något av ovanstående fel uppstår kontrollerar du att servern som skickar eller tar emot e-post har TLS 1.2 aktiverat genom att kontrollera följande registernycklar:</span><span class="sxs-lookup"><span data-stu-id="c335a-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="c335a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="c335a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="c335a-113">Om du gör någon ändring i registernycklarna ovan för att aktivera TLS 1.2 startar du om servern för att ändringarna ska börja gälla.</span><span class="sxs-lookup"><span data-stu-id="c335a-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="c335a-114">Kontrollera också att du har de senaste Windows- och Exchange-uppdateringarna installerade.</span><span class="sxs-lookup"><span data-stu-id="c335a-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="c335a-115">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="c335a-115">For more information, see:</span></span>

- [<span data-ttu-id="c335a-116">TLS-vägledning för Exchange Server, del 1: För förbereda för TLS 1.2 – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="c335a-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="c335a-117">Exchange Server TLS-vägledning Del 2: Aktivera TLS 1.2 och Identifiera klienter som inte använder det – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="c335a-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="c335a-118">Förstå e-postscenarier om det inte går att komma överens om TLS-versioner med Exchange Online – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="c335a-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
