---
title: Logga in på Windows 10 utan att använda ett lösenord
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830564"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="3331f-102">Logga in på Windows 10 utan att använda ett lösenord</span><span class="sxs-lookup"><span data-stu-id="3331f-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="3331f-103">Om du vill undvika att behöva ange ett lösenord vid start av Windows rekommenderar vi att du använder ett av de säkra inloggningsalternativen i Windows Hello, till exempel pin-kod, ansiktsigenkänning eller fingeravtryck, om sådana finns tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="3331f-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="3331f-104">Om du verkligen vill inaktivera säker inloggning kan du läsa instruktionerna "Logga in automatiskt på Windows 10" nedan.</span><span class="sxs-lookup"><span data-stu-id="3331f-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="3331f-105">**Säkra Windows Hello-alternativ till kontolösenordet**</span><span class="sxs-lookup"><span data-stu-id="3331f-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="3331f-106">Gå till **Inställningar > Konton > Inloggningsalternativ (eller** klicka [här](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="3331f-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="3331f-107">Tillgängliga inloggningsalternativ visas.</span><span class="sxs-lookup"><span data-stu-id="3331f-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="3331f-108">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="3331f-108">For example:</span></span>

![Inloggningsalternativ.](media/sign-in-options.png)

<span data-ttu-id="3331f-110">Konfigurera det genom att klicka eller trycka på något av alternativen.</span><span class="sxs-lookup"><span data-stu-id="3331f-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="3331f-111">Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösenord.</span><span class="sxs-lookup"><span data-stu-id="3331f-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="3331f-112">**Logga in automatiskt på Windows 10**</span><span class="sxs-lookup"><span data-stu-id="3331f-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="3331f-113">**Obs!** Automatisk inloggning är praktiskt, men innebär en säkerhetsrisk, särskilt om datorn är tillgänglig för flera personer.</span><span class="sxs-lookup"><span data-stu-id="3331f-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="3331f-114">Klicka eller tryck på **Start-knappen** i Aktivitetsfältet.</span><span class="sxs-lookup"><span data-stu-id="3331f-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="3331f-115">Skriv **netplwiz** och tryck på Retur för att öppna fönstret Användarkonton.</span><span class="sxs-lookup"><span data-stu-id="3331f-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="3331f-116">I **Användarkonton** klickar du på det konto som du vill logga in på automatiskt när Windows startar.</span><span class="sxs-lookup"><span data-stu-id="3331f-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="3331f-117">Avmarkera kryssrutan "Användare måste ange ett användarnamn och lösenord för att kunna använda den här datorn".</span><span class="sxs-lookup"><span data-stu-id="3331f-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Användarna måste ange ett alternativ för användarnamn och lösenord.](media/users-must-enter-username.png)

5. <span data-ttu-id="3331f-119">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="3331f-119">Click **OK**.</span></span> <span data-ttu-id="3331f-120">Du uppmanas att ange och bekräfta lösenordet för det konto som du valt.</span><span class="sxs-lookup"><span data-stu-id="3331f-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="3331f-121">Slutför genom att klicka på **OK.**</span><span class="sxs-lookup"><span data-stu-id="3331f-121">Click **OK** to finish.</span></span> <span data-ttu-id="3331f-122">Nästa gång Windows 10 startar loggas det automatiskt in på det konto som du har valt.</span><span class="sxs-lookup"><span data-stu-id="3331f-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
