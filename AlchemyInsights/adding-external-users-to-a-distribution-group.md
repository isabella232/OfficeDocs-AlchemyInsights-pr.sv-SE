---
title: Lägga till externa användare till en distributionsgrupp
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494545"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="f1223-102">Lägga till externa användare till en distributionsgrupp?</span><span class="sxs-lookup"><span data-stu-id="f1223-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="f1223-103">Lägga till en extern kontakt till en Distribution grupp (GD) är en process i steg 2:</span><span class="sxs-lookup"><span data-stu-id="f1223-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="f1223-104">Skapa en e-kontakt för externa användare:</span><span class="sxs-lookup"><span data-stu-id="f1223-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="f1223-105">Gå till **användare**i administratörscenter, > [sidan](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="f1223-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="f1223-106">Välj **Lägg till en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="f1223-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="f1223-107">Ange information om kontakten och välj **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="f1223-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="f1223-108">Lägg till e-kontakt i din DG:</span><span class="sxs-lookup"><span data-stu-id="f1223-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="f1223-109">Gå till **grupper**i administratörscenter, > [grupper](https://admin.microsoft.com/adminportal/home#/groups) -sidan.</span><span class="sxs-lookup"><span data-stu-id="f1223-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="f1223-110">Hitta DG som du vill lägga till den externa användaren till och markera den för att öppna dialogrutan Redigera.</span><span class="sxs-lookup"><span data-stu-id="f1223-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="f1223-111">Välj **Visa alla och hantera medlemmar**på fliken **medlemmar** .</span><span class="sxs-lookup"><span data-stu-id="f1223-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="f1223-112">Välj **Lägg till medlemmar**.</span><span class="sxs-lookup"><span data-stu-id="f1223-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="f1223-113">Välj e-kontakt som du skapade i föregående steg och välj sedan **Spara**.</span><span class="sxs-lookup"><span data-stu-id="f1223-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="f1223-114">Om efter följande externa användare kan inte skicka e-post till GD eller inte ta emot e-postmeddelanden från den, kan det bero på att GD har markerats för att endast tillåta e-postmeddelanden från interna användare.</span><span class="sxs-lookup"><span data-stu-id="f1223-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="f1223-115">Du kan kontrollera konfigurationen och åtgärda det följa instruktionerna [här](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="f1223-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="f1223-116">**Observera:** Dessa instruktioner gäller inte om din grupp är ”Office 365-grupp” i stället för ”distributionsgrupp”.</span><span class="sxs-lookup"><span data-stu-id="f1223-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="f1223-117">Om så är fallet kan du lägga till den externa användaren direkt till gruppen från Outlook.</span><span class="sxs-lookup"><span data-stu-id="f1223-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="f1223-118">Mer information om Office 365-grupper gäster och instruktioner för att lägga till externa gäster kan hittas i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="f1223-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  