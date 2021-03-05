---
title: Lösenordssynkronisering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483085"
---
# <a name="password-synchronization"></a><span data-ttu-id="e264b-102">Lösenordssynkronisering</span><span class="sxs-lookup"><span data-stu-id="e264b-102">Password synchronization</span></span>

<span data-ttu-id="e264b-103">**Synkronisering av lösenordshashar fungerar inte alls**</span><span class="sxs-lookup"><span data-stu-id="e264b-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="e264b-104">Några vanliga problem som kunder stöter på när synkronisering av lösenordshashar inte fungerar är:</span><span class="sxs-lookup"><span data-stu-id="e264b-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="e264b-105">Det Active Directory-konto som används av Azure AD Connect  för att  kommunicera med lokalt Active Directory beviljas inte behörigheten Replikera katalogändringar och Replikera katalogändringar alla, vilket krävs för lösenordssynkronisering – Du måste åtgärda detta genom att tilldela behörigheterna till Active Directory-kontot.</span><span class="sxs-lookup"><span data-stu-id="e264b-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="e264b-106">Synkronisering av lösenordshashar inaktiveras när en  administratör har ändrat User Sign-In-metoden från lösenordssynkronisering till ett annat alternativ,  till exempel Federation med **AD FS** i Azure AD Connect-guiden – Du kan åtgärda det genom att aktivera synkroniseringsfunktionen för lösenordshashar på nytt i guiden Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e264b-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="e264b-107">Anslutningsproblem med lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e264b-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="e264b-108">Vissa domänkontrollanter kan till exempel inte nås av [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect, eller så blockeras de portar som krävs av brandväggen – Du måste åtgärda detta genom att säkerställa att anslutningen mellan Azure AD Connect-servern och den lokala Active Directory fungerar som den ska.</span><span class="sxs-lookup"><span data-stu-id="e264b-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="e264b-109">Azure AD Connect-servern är för närvarande i mellanlagringsläge, vilket gör att servern inte kan [lösenordshashar](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)- För att felsöka problemet följer du stegen som beskrivs i avsnittet Felsöka lösenordssynkronisering med Azure AD Connect-synkronisering – Inga lösenord synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="e264b-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="e264b-110">**Synkronisering av lösenordshashar fungerar inte för vissa av mina användare**</span><span class="sxs-lookup"><span data-stu-id="e264b-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="e264b-111">Om du lade märke till att lösenordshashar  inte synkroniseras för en användare kan du använda felsökningsaktiviteten i Azure AD Connect för att undersöka och lösa problemet.</span><span class="sxs-lookup"><span data-stu-id="e264b-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="e264b-112">Utför följande uppgifter:</span><span class="sxs-lookup"><span data-stu-id="e264b-112">Perform the following tasks:</span></span>

    <span data-ttu-id="e264b-113">a.</span><span class="sxs-lookup"><span data-stu-id="e264b-113">a.</span></span> [<span data-ttu-id="e264b-114">Köra felsökningsaktiviteten i guiden</span><span class="sxs-lookup"><span data-stu-id="e264b-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="e264b-115">b.</span><span class="sxs-lookup"><span data-stu-id="e264b-115">b.</span></span> [<span data-ttu-id="e264b-116">Använd cmdleten för felsökning för att undersöka problemet med synkronisering av lösenordshashar för en viss användning</span><span class="sxs-lookup"><span data-stu-id="e264b-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="e264b-117">Det lokala Active Directory-användarobjektet är aktiverat för **användaren måste ändra lösenord vid nästa inloggningsalternativ.**</span><span class="sxs-lookup"><span data-stu-id="e264b-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="e264b-118">När det här alternativet är aktiverat tilldelas användaren ett tillfälligt lösenord och uppmanas att ändra lösenordet vid nästa inloggning.</span><span class="sxs-lookup"><span data-stu-id="e264b-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="e264b-119">Azure AD Connect synkroniserar inte tillfälliga lösenord med Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e264b-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="e264b-120">Lös problemet genom att utföra någon av följande uppgifter:</span><span class="sxs-lookup"><span data-stu-id="e264b-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="e264b-121">Be användaren att logga in på det lokala programmet (till exempel Windows-skrivbordet) och ändra lösenordet.</span><span class="sxs-lookup"><span data-stu-id="e264b-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="e264b-122">Det nya lösenordet synkroniseras till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e264b-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="e264b-123">Be en administratör uppdatera användarens lösenord utan att aktivera alternativet Användaren måste ändra lösenordet vid nästa inloggning och dela det nya lösenordet med användaren.</span><span class="sxs-lookup"><span data-stu-id="e264b-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="e264b-124">Det lokala Active Directory-användarobjektet är inte **korrekt konfigurerat för objektsynkronisering** eller lösenordssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="e264b-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="e264b-125">För att felsöka det här problemet följer du stegen som beskrivs i Felsöka synkronisering [av lösenordshashar med Azure AD Connect-synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="e264b-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







