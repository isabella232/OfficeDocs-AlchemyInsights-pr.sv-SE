---
title: S/MIME i Outlook på webben
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511526"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="1c7b3-102">Kryptera e-postmeddelanden i Outlook</span><span class="sxs-lookup"><span data-stu-id="1c7b3-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="1c7b3-103">Microsoft 365 Message Encryption bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="1c7b3-104">Om din prenumeration innehåller Azure Rights Management eller Azure Information Protection **behöver du inte vidta några åtgärder för att manuellt aktivera eller aktivera** Rights Management Service.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="1c7b3-105">Baserat på feedback från kunder kommer vi inte längre att aktivera Exchange-regler för e-postflöde för att automatiskt kryptera utgående e-post som innehåller viss typ av känslig information i din klientorganisation som standard.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="1c7b3-106">I stället ger vi detaljerade instruktioner om hur ni själva kan göra det.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="1c7b3-107">Mer information om hur du skapar en transportregel för att kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="1c7b3-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="1c7b3-108">Om du använder Outlook på webben (tidigare **OWA**): När du skriver ett e-postmeddelande klickar du bara på **Skydda** i OWA.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="1c7b3-109">Detta gäller behörigheten "Vidarebefordra inte".</span><span class="sxs-lookup"><span data-stu-id="1c7b3-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="1c7b3-110">Klicka på **Ändra behörighet** och välj **Kryptera** om du bara vill kryptera meddelandet.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="1c7b3-111">Om du använder **Outlook-klienten**: Om du vill skicka ett krypterat meddelande från Outlook 2013 eller 2016 eller Outlook 2016 för Mac väljer du **Options**  >  **Alternativbehörigheter**och väljer sedan det skyddsalternativ du behöver.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="1c7b3-112">Om du **vill kryptera alla e-postmeddelanden** som skickas till vissa mottagare eller externa partnerorganisationer automatiskt måste du skapa en transportregel för e-postflöde i Administrationscenter för Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c7b3-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="1c7b3-113">Detaljerade instruktioner finns i [den här supportartikeln](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="1c7b3-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

