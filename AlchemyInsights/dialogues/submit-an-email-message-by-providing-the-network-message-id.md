---
title: Skicka ett e-postmeddelande genom att ange nätverksmeddelande-ID
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695380"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="0ed02-102">Skicka ett e-postmeddelande genom att ange nätverksmeddelande-ID</span><span class="sxs-lookup"><span data-stu-id="0ed02-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="0ed02-103">Välj **E-post och**  Nätverksmeddelande-ID i den nya **utfällningen av inskickade meddelanden.**</span><span class="sxs-lookup"><span data-stu-id="0ed02-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="0ed02-104">Följ de här anvisningarna för att hitta meddelande-ID för ett e-postmeddelande i Outlook:</span><span class="sxs-lookup"><span data-stu-id="0ed02-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="0ed02-105">Dubbelklicka på e-postmeddelandet för att öppna det.</span><span class="sxs-lookup"><span data-stu-id="0ed02-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="0ed02-106">Välj   >  **Filegenskaper.**</span><span class="sxs-lookup"><span data-stu-id="0ed02-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="0ed02-107">Öppna Anteckningar eller ett tomt Word-dokument och kopiera och klistra sedan in innehållet i **rutan Internetrubriker** i det öppna dokumentet för bättre synlighet.</span><span class="sxs-lookup"><span data-stu-id="0ed02-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="0ed02-108">Leta reda **på fältet X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="0ed02-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="0ed02-109">Värdet efter : är **det** ID du behöver för din inskicking.</span><span class="sxs-lookup"><span data-stu-id="0ed02-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="0ed02-110">Välj **Markera** alla under Mottagare om e-postmeddelandet hamnar i skräppostmappen för alla mottagare av det **här e-postmeddelandet.**</span><span class="sxs-lookup"><span data-stu-id="0ed02-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="0ed02-111">Om inte, väljer du bara den användare som rapporterade problemet.</span><span class="sxs-lookup"><span data-stu-id="0ed02-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="0ed02-112">Om **du väljer** Borde ha blockerats under Orsak för inskickning anger du om meddelandet ska ha blockerats som **skräppost,** nätfiske eller skadlig kod och väljer sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="0ed02-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="0ed02-113">Om du vill veta mer kan du läsa om hur du skickar misstänkt [skräppost, phish, URL:er och filer till Microsoft för genomsökning.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="0ed02-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
