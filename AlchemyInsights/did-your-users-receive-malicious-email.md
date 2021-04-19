---
title: Har användarna fått skadlig e-post
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815264"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="27883-102">Har användarna fått skadlig e-post?</span><span class="sxs-lookup"><span data-stu-id="27883-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="27883-103">Nu kan du rapportera skadlig e-post till Microsoft med hjälp [Administratörsinlämningar i Säkerhets- och efterlevnadscenter](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="27883-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="27883-104">Meddelanden som skickas in [-administratörsinlämningar](https://sip.protection.office.com/reportsubmission) genomsöks och följande resultat visas i **information** som utfälld:</span><span class="sxs-lookup"><span data-stu-id="27883-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="27883-105">Om avsändarens e-postautentisering misslyckades vid leveransen.</span><span class="sxs-lookup"><span data-stu-id="27883-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="27883-106">Information om politiska träffar som kan ha påverkat eller åsidosatt bedömningen av ett meddelande.</span><span class="sxs-lookup"><span data-stu-id="27883-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="27883-107">Aktuella detonationsresultat för att se om webbadresserna eller filerna i meddelandet var skadliga eller inte.</span><span class="sxs-lookup"><span data-stu-id="27883-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="27883-108">Feedback från klassare</span><span class="sxs-lookup"><span data-stu-id="27883-108">Feedback from graders</span></span>

<span data-ttu-id="27883-109">Om en åsidosättning hittades bör omskanningen slutföras på några minuter.</span><span class="sxs-lookup"><span data-stu-id="27883-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="27883-110">Om det inte uppstod något problem med e-postautentisering eller om leveransen inte påverkades av en åsidosättning, kan det ta upp till en dag för feedbacken från klasserna.</span><span class="sxs-lookup"><span data-stu-id="27883-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="27883-111">Om du inte håller med den slutliga domen om ett meddelande, URL eller fil (blockerad kontra inte blockerad), skicka meddelandet igen efter en dag för att skanna igen.</span><span class="sxs-lookup"><span data-stu-id="27883-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="27883-112">Sannolikheten är stor för att domen skulle förändras efter att ha skickat meddelandet igen.</span><span class="sxs-lookup"><span data-stu-id="27883-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="27883-113">Under tiden kan du ta bort skadlig e-post från användarnas inkorgar genom att följa anvisningarna [i den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="27883-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="27883-114">Kunder med Microsoft Defender för Office 365 kan:</span><span class="sxs-lookup"><span data-stu-id="27883-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="27883-115">använder [Utforskaren för att hitta och ta bort misstänkta e-postmeddelanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="27883-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="27883-116">[använder du Säkra länkar för att blockera åtkomst](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) till en skadlig URL</span><span class="sxs-lookup"><span data-stu-id="27883-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="27883-117">spåra användare som har klickat på och kommit åt skadliga URL:er: [Visa nätfiske-URL och klicka på bedömningsdata](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="27883-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="27883-118">manuellt [starta en automatiserad undersökning](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="27883-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="27883-119">Du kan också skydda mot skadliga filer och URL-adresser genom att följa anvisningarna i [Skydd mot skadliga URL:er och filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="27883-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>