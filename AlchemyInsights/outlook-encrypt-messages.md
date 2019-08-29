---
title: S/MIME i Outlook på webben
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666858"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="b7bf1-102">Kryptera e-postmeddelanden i Outlook</span><span class="sxs-lookup"><span data-stu-id="b7bf1-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="b7bf1-103">Office 365-meddelandekryptering är byggd på Microsoft Azure Rights Management (Azure RMS), som är en del av informationsskydd i Azure.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="b7bf1-104">Om prenumerationen innehåller Azure Rights Management eller Azure informationsskydd, **du behöver inte vidta några åtgärder för att manuellt aktivera eller aktivera** tjänsten Rights Management.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="b7bf1-105">Baserat på kundernas feedback kommer vi inte längre att aktivera Exchange e-flöde regler att automatiskt kryptera utgående e-post som innehåller en viss typ av känslig information i din innehavare som standard.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="b7bf1-106">I stället vi tillhandahåller detaljerade instruktioner om hur du gör det yourselves.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="b7bf1-107">Mer information om hur du skapar en transportregel om du vill kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="b7bf1-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="b7bf1-108">Om du använder Outlook på webben (tidigare **OWA**): när du skriver ett e-postmeddelande, bara klicka på **skydda** i OWA.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="b7bf1-109">”Gör inte framåt” behörighet gäller.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="b7bf1-110">Klicka på **Ändra behörighet** och välj **kryptera** endast kryptera meddelandet.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="b7bf1-111">Om du använder **Outlook-klienten**: Välj **Alternativ**om du vill skicka ett krypterat meddelande från Outlook 2013 och 2016 eller Outlook 2016 för Mac, > **behörigheter**och sedan välja alternativet skydd du behöver.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="b7bf1-112">Att **automatiskt kryptera all e-post** skickas till vissa mottagare eller externa partnerorganisationer, måste du skapa en regel för e-post flöde transport i Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="b7bf1-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="b7bf1-113">Detaljerade anvisningar finns i [denna artikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="b7bf1-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

