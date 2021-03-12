---
title: Skicka ett e-postmeddelande genom att ange nätverkets meddelande-ID
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748207"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="8a11d-102">Skicka ett e-postmeddelande genom att ange nätverkets meddelande-ID</span><span class="sxs-lookup"><span data-stu-id="8a11d-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="8a11d-103">Välj **E-post och** Nätverksmeddelande-ID i **den** **utfäll plats som visas för ny inskickning.**</span><span class="sxs-lookup"><span data-stu-id="8a11d-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="8a11d-104">Följ de här anvisningarna för att hitta meddelande-ID för ett e-postmeddelande i Outlook:</span><span class="sxs-lookup"><span data-stu-id="8a11d-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="8a11d-105">Dubbelklicka på e-postmeddelandet för att öppna det.</span><span class="sxs-lookup"><span data-stu-id="8a11d-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="8a11d-106">Välj   >  **Filegenskaper**.</span><span class="sxs-lookup"><span data-stu-id="8a11d-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="8a11d-107">Öppna Anteckningar eller ett tomt Word-dokument och kopiera och klistra sedan in innehållet från rutan **Internetrubriker** i det öppna dokumentet för bättre synlighet.</span><span class="sxs-lookup"><span data-stu-id="8a11d-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="8a11d-108">Leta reda **på fältet X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="8a11d-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="8a11d-109">Värdet efter den **: är det** ID du behöver för din inskicking.</span><span class="sxs-lookup"><span data-stu-id="8a11d-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="8a11d-110">Om e-postmeddelandet hamnar i skräppostmappen för alla mottagare av det här e-postmeddelandet väljer du Markera alla under **Mottagare.**</span><span class="sxs-lookup"><span data-stu-id="8a11d-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="8a11d-111">Annars väljer du bara den användare som rapporterade problemet.</span><span class="sxs-lookup"><span data-stu-id="8a11d-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="8a11d-112">Om **du väljer** Borde ha blockerats under Orsak till inskickning anger du om meddelandet ska ha blockerats som **skräppost,** nätfiske eller skadlig kod och väljer sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="8a11d-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="8a11d-113">Mer information finns i [Så här skickar du misstänkt skräppost, nättr ut, URL:er och filer till Microsoft för genomsökning.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="8a11d-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
