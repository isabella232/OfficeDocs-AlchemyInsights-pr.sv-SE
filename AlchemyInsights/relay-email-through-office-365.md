---
title: Vidarebefordra e-post via Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 727fa38233697c778caa9325b2671501cb75d5fd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510734"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="30e9b-102">Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post</span><span class="sxs-lookup"><span data-stu-id="30e9b-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="30e9b-103">Mer information om alternativ och anvisningar finns i [Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post med hjälp av Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="30e9b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="30e9b-104">**Obs!** Om du har en enhet eller ett program som nyligen har slutat fungera vill vi göra dig uppmärksam på att vi nyligen har börjat [inaktivera 3DES-chiffreringen](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) som planerat.</span><span class="sxs-lookup"><span data-stu-id="30e9b-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="30e9b-105">Om du vill se påverkade enheter går du till rapporten [SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="30e9b-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="30e9b-106">Vanliga fel kan vara: Autentiseringsfel, TLS-fel, felaktig chiffreringsalgoritm, algoritmkonflikt eller avbruten anslutning.</span><span class="sxs-lookup"><span data-stu-id="30e9b-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="30e9b-107">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="30e9b-107">To resolve the issue:</span></span>
 - <span data-ttu-id="30e9b-108">**Windows Server 2003 IIS SMTP fungerar inte längre – en nyare version av Windows krävs.**</span><span class="sxs-lookup"><span data-stu-id="30e9b-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="30e9b-109">Kontakta leverantören för programmet eller enheten och kontrollera om en modern chiffrering stöds eller om det finns en uppdatering.</span><span class="sxs-lookup"><span data-stu-id="30e9b-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
