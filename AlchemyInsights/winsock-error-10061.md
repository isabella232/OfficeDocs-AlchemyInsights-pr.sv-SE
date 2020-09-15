---
title: 1554 Winsock-fel 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698880"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="32b82-102">Winsock-fel 10061</span><span class="sxs-lookup"><span data-stu-id="32b82-102">Winsock error 10061</span></span>

<span data-ttu-id="32b82-103">Den här felkoden innebär att Microsoft inte kunde upprätta en TCP-socket (anslutning) med mål värden.</span><span class="sxs-lookup"><span data-stu-id="32b82-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="32b82-104">Den mest sannolika orsaken till det här felet är ett problem med din brand Väggs konfiguration.</span><span class="sxs-lookup"><span data-stu-id="32b82-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="32b82-105">Åtgärda problemet genom att kontrol lera följande:</span><span class="sxs-lookup"><span data-stu-id="32b82-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="32b82-106">Kontrol lera din brand Väggs konfiguration med informationen i [Microsoft 365 URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="32b82-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="32b82-107">Om felet är specifikt för Exchange Online Protection (EOP), bör du tidigare meddelas om [Exchange Online Protection IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="32b82-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="32b82-108">Kontrol lera att Internet leverantören inte blockerar porten.</span><span class="sxs-lookup"><span data-stu-id="32b82-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="32b82-109">Kontrol lera inställningarna för smart värd och mål server i dina kontakter.</span><span class="sxs-lookup"><span data-stu-id="32b82-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="32b82-110">Observera att Microsoft 365 inte blockerar *inkommande* anslutningar på det här sättet.</span><span class="sxs-lookup"><span data-stu-id="32b82-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
