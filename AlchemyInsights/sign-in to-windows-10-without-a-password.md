---
title: Logga in på Windows 10 utan att använda ett lösenord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588298"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="d69ea-102">Logga in på Windows 10 utan att använda ett lösenord</span><span class="sxs-lookup"><span data-stu-id="d69ea-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="d69ea-103">För att undvika att behöva skriva ett lösenord vid start av Windows rekommenderar vi att du använder något av alternativen för säker inloggning i Windows Hello, till exempel en PIN-kod, ansiktsigenkänning eller fingeravtryck, om tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="d69ea-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="d69ea-104">Om du verkligen vill inaktivera säker inloggning läser du instruktionerna "Logga automatiskt in i Windows 10" nedan.</span><span class="sxs-lookup"><span data-stu-id="d69ea-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="d69ea-105">**Säkra Windows Hello-alternativ till kontolösenordet**</span><span class="sxs-lookup"><span data-stu-id="d69ea-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="d69ea-106">Gå till **Inställningar > konton > inloggningsalternativ** (eller klicka [här).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="d69ea-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d69ea-107">Tillgängliga inloggningsalternativ visas.</span><span class="sxs-lookup"><span data-stu-id="d69ea-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="d69ea-108">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="d69ea-108">For example:</span></span>

![Inloggningsalternativ.](media/sign-in-options.png)

<span data-ttu-id="d69ea-110">Klicka eller tryck på något av alternativen för att konfigurera det.</span><span class="sxs-lookup"><span data-stu-id="d69ea-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="d69ea-111">Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösenord.</span><span class="sxs-lookup"><span data-stu-id="d69ea-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="d69ea-112">**Logga in automatiskt i Windows 10**</span><span class="sxs-lookup"><span data-stu-id="d69ea-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="d69ea-113">**Automatisk**inloggning är praktiskt, men introducerar en säkerhetsrisk, särskilt om datorn är tillgänglig för flera personer.</span><span class="sxs-lookup"><span data-stu-id="d69ea-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="d69ea-114">Klicka eller tryck på **Start-knappen** i Aktivitetsfältet.</span><span class="sxs-lookup"><span data-stu-id="d69ea-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="d69ea-115">Skriv **netplwiz** och tryck på Retur-tangenten för att öppna fönstret Användarkonton.</span><span class="sxs-lookup"><span data-stu-id="d69ea-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="d69ea-116">I **Användarkonton**klickar du på det konto som du vill logga in automatiskt på när Windows startar.</span><span class="sxs-lookup"><span data-stu-id="d69ea-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="d69ea-117">Avmarkera kryssrutan "Användare måste ange ett användarnamn och lösenord för att använda den här datorn".</span><span class="sxs-lookup"><span data-stu-id="d69ea-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Användare måste ange ett användarnamn och lösenord alternativ.](media/users-must-enter-username.png)

5. <span data-ttu-id="d69ea-119">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="d69ea-119">Click **OK**.</span></span> <span data-ttu-id="d69ea-120">Du kommer att bli ombedd att ange och bekräfta lösenordet för det valda kontot.</span><span class="sxs-lookup"><span data-stu-id="d69ea-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="d69ea-121">Klicka på **OK** för att avsluta.</span><span class="sxs-lookup"><span data-stu-id="d69ea-121">Click **OK** to finish.</span></span> <span data-ttu-id="d69ea-122">Nästa gång Windows 10 startar loggas det automatiskt in på det konto du valde.</span><span class="sxs-lookup"><span data-stu-id="d69ea-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
