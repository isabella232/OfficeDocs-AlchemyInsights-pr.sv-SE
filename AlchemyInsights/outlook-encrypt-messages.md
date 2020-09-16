---
title: S/MIME i Outlook på webben
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772316"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="673bb-102">Kryptera e-postmeddelanden i Outlook</span><span class="sxs-lookup"><span data-stu-id="673bb-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="673bb-103">Microsoft 365 meddelande kryptering bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure information Protection.</span><span class="sxs-lookup"><span data-stu-id="673bb-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="673bb-104">Om ditt abonnemang inkluderar Azure Rights Management eller Azure information Protection **behöver du inte vidta några åtgärder för att aktivera eller inaktivera** Rights Management-tjänsten manuellt.</span><span class="sxs-lookup"><span data-stu-id="673bb-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="673bb-105">Baserat på feedback från kunder kommer vi inte längre att aktivera regler för Exchange-postflöde för att automatiskt kryptera utgående e-post som innehåller viss typ av känslig information i klient organisationen.</span><span class="sxs-lookup"><span data-stu-id="673bb-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="673bb-106">I stället tillhandahåller vi detaljerade anvisningar om hur du gör det hör dock.</span><span class="sxs-lookup"><span data-stu-id="673bb-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="673bb-107">Mer information om hur du skapar en transport regel för att kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="673bb-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="673bb-108">Om du använder Outlook på webben (tidigare **OWA**): när du skriver ett e-postmeddelande klickar du helt enkelt på **skydda** i OWA.</span><span class="sxs-lookup"><span data-stu-id="673bb-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="673bb-109">Detta tillämpar behörigheten "Vidarekoppla inte".</span><span class="sxs-lookup"><span data-stu-id="673bb-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="673bb-110">Klicka på **Ändra behörighet** och välj **kryptera** för att kryptera meddelandet.</span><span class="sxs-lookup"><span data-stu-id="673bb-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="673bb-111">Om du använder **Outlook-klienten**: för att skicka ett krypterat meddelande från Outlook 2013 eller 2016, eller Outlook 2016 för Mac, väljer du **alternativ**  >  **behörigheter**och väljer sedan det skydds alternativ du behöver.</span><span class="sxs-lookup"><span data-stu-id="673bb-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="673bb-112">För att **automatiskt kryptera alla e-postmeddelanden** som skickas till vissa mottagare eller externa partner organisationer måste du skapa en regel för e-postflödes transport i administrations centret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="673bb-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="673bb-113">Detaljerade anvisningar finns i [den här Support artikeln](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="673bb-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

