---
title: Lägga till eller ta bort ett ombud i Outlook för Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573811"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="a810c-102">Lägga till eller ta bort ett ombud i Outlook för Windows</span><span class="sxs-lookup"><span data-stu-id="a810c-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="a810c-103">Så här lägger du till ett ombud i Outlook för Windows:</span><span class="sxs-lookup"><span data-stu-id="a810c-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="a810c-104">Klicka på fliken **Arkiv** följt av **konto inställningar** och välj sedan **ombud**.</span><span class="sxs-lookup"><span data-stu-id="a810c-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="a810c-105">Klicka på **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="a810c-105">Click on **Add**.</span></span> <span data-ttu-id="a810c-106">Om **Lägg till** inte visas kan det bero på att det inte finns en aktiv anslutning mellan Outlook och Exchange.</span><span class="sxs-lookup"><span data-stu-id="a810c-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="a810c-107">I statusfältet i Outlook visas anslutnings status.</span><span class="sxs-lookup"><span data-stu-id="a810c-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="a810c-108">Skriv namnet på den person du vill ange som ombud, eller Sök och välj namnet i listan Sök resultat.</span><span class="sxs-lookup"><span data-stu-id="a810c-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a810c-109">Ombudet måste vara en person i organisationens globala adress lista (GAL).</span><span class="sxs-lookup"><span data-stu-id="a810c-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="a810c-110">Klicka på **Lägg till** följt av **OK**.</span><span class="sxs-lookup"><span data-stu-id="a810c-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="a810c-111">Godkänn standardinställningarna i dialog rutan **behörigheter för ombud** eller Välj anpassade åtkomst nivåer för Exchange-mappar.</span><span class="sxs-lookup"><span data-stu-id="a810c-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="a810c-112">Om ett ombud behöver behörighet att endast arbeta med Mötes förfrågningar och svar är det tillräckligt med de förvalda behörighets inställningarna, till exempel **ombud** .</span><span class="sxs-lookup"><span data-stu-id="a810c-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="a810c-113">Du kan lämna behörighets inställningen för **Inkorgen** **.**</span><span class="sxs-lookup"><span data-stu-id="a810c-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="a810c-114">Mötes förfrågningar och svar skickas direkt till ombudets inkorg.</span><span class="sxs-lookup"><span data-stu-id="a810c-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a810c-115">Som standard tillåts ombudet **(kan läsa, skapa och ändra objekt)** behörighet till mappen **kalender** .</span><span class="sxs-lookup"><span data-stu-id="a810c-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="a810c-116">När ombudet svarar på ett möte åt dig läggs det automatiskt till i mappen **kalender** .</span><span class="sxs-lookup"><span data-stu-id="a810c-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="a810c-117">Om du vill skicka ett meddelande om du vill meddela ombudet om de ändrade behörigheterna markerar du kryss rutan **Skicka automatiskt ett meddelande till ombudet om att sammanfatta dessa behörigheter** .</span><span class="sxs-lookup"><span data-stu-id="a810c-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="a810c-118">Markera kryss rutan **ombud kan se mina privata objekt** om du vill.</span><span class="sxs-lookup"><span data-stu-id="a810c-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="a810c-119">Den här inställningen påverkar alla Exchange-mappar.</span><span class="sxs-lookup"><span data-stu-id="a810c-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="a810c-120">Detta inkluderar all e-post, kontakter, kalender, uppgifter, anteckningar och journalmallar.</span><span class="sxs-lookup"><span data-stu-id="a810c-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="a810c-121">Det finns inget sätt att bevilja åtkomst till privata objekt i endast angivna mappar.</span><span class="sxs-lookup"><span data-stu-id="a810c-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="a810c-122">Välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="a810c-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="a810c-123">Meddelanden som skickas med behörigheter för skicka i uppdrag inkluderar både ombudets och deras namn bredvid **från**.</span><span class="sxs-lookup"><span data-stu-id="a810c-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="a810c-124">När ett meddelande skickas med skicka som-behörighet visas bara ditt namn.</span><span class="sxs-lookup"><span data-stu-id="a810c-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="a810c-125">När du lägger till någon som ombud kan de lägga till din Exchange-postlåda i sin Outlook-profil.</span><span class="sxs-lookup"><span data-stu-id="a810c-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="a810c-126">Anvisningar finns i [hantera en annan persons e-post och Kalender objekt](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="a810c-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="a810c-127">Så här tar du bort ett ombud i Outlook för Windows:</span><span class="sxs-lookup"><span data-stu-id="a810c-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="a810c-128">Klicka på fliken **Arkiv** .</span><span class="sxs-lookup"><span data-stu-id="a810c-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="a810c-129">Klicka på **konto inställningar** följt av **ombuds åtkomst**.</span><span class="sxs-lookup"><span data-stu-id="a810c-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="a810c-130">Välj namnet på det ombud som du vill ändra behörigheter för och klicka sedan på **ta bort** följt av **OK**.</span><span class="sxs-lookup"><span data-stu-id="a810c-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
