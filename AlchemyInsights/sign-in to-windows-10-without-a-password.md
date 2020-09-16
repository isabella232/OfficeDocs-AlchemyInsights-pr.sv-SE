---
title: Logga in i Windows 10 utan lösen ord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719971"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="9fbc6-102">Logga in i Windows 10 utan lösen ord</span><span class="sxs-lookup"><span data-stu-id="9fbc6-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="9fbc6-103">För att undvika att behöva ange ett lösen ord när du startar Windows rekommenderar vi att du använder ett av de säkra inloggnings alternativen för Windows Hello, till exempel en PIN-kod, en ansikts igenkänning eller ett finger avtryck, om det är tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="9fbc6-104">Om du vill inaktivera säker inloggning kan du läsa anvisningarna "logga in automatiskt på Windows 10" nedan.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="9fbc6-105">**Säkra Windows Hello-alternativ till konto lösen ordet**</span><span class="sxs-lookup"><span data-stu-id="9fbc6-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="9fbc6-106">Gå till **inställningar > konton > inloggnings alternativ** (eller klicka [här](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="9fbc6-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="9fbc6-107">Tillgängliga inloggnings alternativ visas.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="9fbc6-108">Ett exempel:</span><span class="sxs-lookup"><span data-stu-id="9fbc6-108">For example:</span></span>

![Inloggnings alternativ.](media/sign-in-options.png)

<span data-ttu-id="9fbc6-110">Klicka eller tryck på ett av alternativen för att konfigurera det.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="9fbc6-111">Nästa gång du startar eller låser upp Windows kan du använda det nya alternativet i stället för ett lösen ord.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="9fbc6-112">**Logga in automatiskt i Windows 10**</span><span class="sxs-lookup"><span data-stu-id="9fbc6-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="9fbc6-113">**Obs!** automatisk inloggning är bekvämt, men introducerar en säkerhets risk, särskilt om din dator är tillgänglig för flera personer.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="9fbc6-114">Klicka eller tryck på **Start** -knappen i aktivitets fältet.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="9fbc6-115">Skriv **netplwiz** och tryck på RETUR för att öppna fönstret användar konton.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="9fbc6-116">I **användar konton**klickar du på det konto som du vill logga in automatiskt på när Windows startas.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="9fbc6-117">Avmarkera kryss rutan "användare måste ange användar namn och lösen ord för att använda den här datorn".</span><span class="sxs-lookup"><span data-stu-id="9fbc6-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Användare måste ange ett användar namn och lösen ord.](media/users-must-enter-username.png)

5. <span data-ttu-id="9fbc6-119">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-119">Click **OK**.</span></span> <span data-ttu-id="9fbc6-120">Du uppmanas att ange och bekräfta lösen ordet för det konto som du har valt.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="9fbc6-121">Klicka på **OK** för att avsluta.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-121">Click **OK** to finish.</span></span> <span data-ttu-id="9fbc6-122">Nästa gång Windows 10 startas loggar det automatiskt in på det konto som du har valt.</span><span class="sxs-lookup"><span data-stu-id="9fbc6-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
