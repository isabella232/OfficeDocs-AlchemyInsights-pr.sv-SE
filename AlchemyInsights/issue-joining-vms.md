---
title: Problem med att ansluta till virtuella datorer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885660"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="cc4ad-102">Problem med att ansluta till virtuella datorer</span><span class="sxs-lookup"><span data-stu-id="cc4ad-102">Issue joining VMs</span></span>

<span data-ttu-id="cc4ad-103">Så här löser du problem som uppstår när du försöker ansluta till virtuella datorer:</span><span class="sxs-lookup"><span data-stu-id="cc4ad-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="cc4ad-104">Försök att logga in med **UPN** -formatet (till exempel "joeuser@contoso.com") i stället för **sAMAccountName** -formatet ("CONTOSO\joeuser").</span><span class="sxs-lookup"><span data-stu-id="cc4ad-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="cc4ad-105">Kontrol lera att du har aktiverat Lösenordssynkronisering enligt anvisningarna i *komma igång* -guiden.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="cc4ad-106">Kontrol lera att det användar konto som påverkas inte är ett externt konto i Azure AD-innehavaren.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="cc4ad-107">Externa användare kan inte logga in på den hanterade domänen eftersom Azure AD Domain Services inte har autentiseringsuppgifter för sådana användar konton.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="cc4ad-108">Om det berörda användar kontot är ett moln-Only-konto kontrollerar du att användarna har ändrat sitt lösen ord efter att du aktiverat Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="cc4ad-109">Det här steget gör att hash-värden för autentiseringsuppgifter krävs för att Azure AD Domain Services ska kunna genereras.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="cc4ad-110">Om de berörda användar kontona synkroniseras från en lokal katalog kontrollerar du att Rekommenderad version av Azure AD Connect har kon figurer ATS för en fullständig synkronisering.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="cc4ad-111">Om problemen kvarstår efter att du har bekräftat steg 4 kör du följande kommandon från synkkabeln:</span><span class="sxs-lookup"><span data-stu-id="cc4ad-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="cc4ad-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="cc4ad-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>