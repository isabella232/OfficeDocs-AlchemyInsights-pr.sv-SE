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
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785213"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="ad5e2-102">Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post</span><span class="sxs-lookup"><span data-stu-id="ad5e2-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="ad5e2-103">Mer information om alternativ och anvisningar finns i [Konfigurera en multifunktionsenhet eller ett multifunktionsprogram för att skicka e-post med hjälp av Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="ad5e2-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="ad5e2-104">**Obs!** Om du har en enhet eller ett program som nyligen har slutat fungera vill vi göra dig uppmärksam på att vi nyligen har börjat [inaktivera 3DES-chiffreringen](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) som planerat.</span><span class="sxs-lookup"><span data-stu-id="ad5e2-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="ad5e2-105">Om du vill se påverkade enheter går du till rapporten [SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ad5e2-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="ad5e2-106">Vanliga fel kan vara: Autentiseringsfel, TLS-fel, felaktig chiffreringsalgoritm, algoritmkonflikt eller avbruten anslutning.</span><span class="sxs-lookup"><span data-stu-id="ad5e2-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="ad5e2-107">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="ad5e2-107">To resolve the issue:</span></span>
 - <span data-ttu-id="ad5e2-108">**Windows Server 2003 IIS SMTP fungerar inte längre – en nyare version av Windows krävs.**</span><span class="sxs-lookup"><span data-stu-id="ad5e2-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="ad5e2-109">Kontakta leverantören för programmet eller enheten och kontrollera om en modern chiffrering stöds eller om det finns en uppdatering.</span><span class="sxs-lookup"><span data-stu-id="ad5e2-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
