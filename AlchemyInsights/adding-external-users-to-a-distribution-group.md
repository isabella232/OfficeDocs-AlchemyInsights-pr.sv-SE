---
title: Lägga till externa användare i en distributionsgrupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910950"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="2f014-102">Lägga till externa användare i en distributionsgrupp</span><span class="sxs-lookup"><span data-stu-id="2f014-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="2f014-103">Att lägga till en extern kontakt i en distributionsgrupp (GD) är en tvåstegsprocess:</span><span class="sxs-lookup"><span data-stu-id="2f014-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="2f014-104">Skapa en e-postkontakt för den externa användaren:</span><span class="sxs-lookup"><span data-stu-id="2f014-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="2f014-105">Gå till sidan[Användares kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i **administrationscentret.** > </span><span class="sxs-lookup"><span data-stu-id="2f014-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="2f014-106">Välj **Lägg till en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="2f014-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="2f014-107">Skriv informationen för kontakten och välj **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="2f014-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="2f014-108">Lägg till e-postkontakten i gd:</span><span class="sxs-lookup"><span data-stu-id="2f014-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="2f014-109">Gå till sidan **Gruppergrupper** > [i](https://admin.microsoft.com/adminportal/home#/groups) administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="2f014-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="2f014-110">Leta reda på det DG som du vill lägga till den externa användaren i och markera det för att öppna redigeringsdialogrutan.</span><span class="sxs-lookup"><span data-stu-id="2f014-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="2f014-111">På fliken **Medlemmar** väljer du **Visa alla och hanterar medlemmar**.</span><span class="sxs-lookup"><span data-stu-id="2f014-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="2f014-112">Välj **Lägg till medlemmar**.</span><span class="sxs-lookup"><span data-stu-id="2f014-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="2f014-113">Markera den e-postkontakt som du skapade i föregående steg och välj sedan **Spara**.</span><span class="sxs-lookup"><span data-stu-id="2f014-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="2f014-114">Om dina externa användare efter att ha följt dessa steg inte kan skicka e-post till GD eller inte får e-postmeddelanden från det, kan det vara så att GD är markerat för att endast tillåta e-postmeddelanden från interna användare.</span><span class="sxs-lookup"><span data-stu-id="2f014-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="2f014-115">Du kan kontrollera den här konfigurationen och åtgärda den efter anvisningarna [här](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="2f014-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="2f014-116">**Anm.:** De här instruktionerna gäller inte om gruppens typ är "Microsoft 365-grupp" i stället för "Distributionsgrupp".</span><span class="sxs-lookup"><span data-stu-id="2f014-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="2f014-117">Om så är fallet kan du lägga till den externa användaren direkt i gruppen från Outlook.</span><span class="sxs-lookup"><span data-stu-id="2f014-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="2f014-118">Detaljerad information om Microsoft 365 Groups gäster samt instruktioner för att lägga till externa gäster finns i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="2f014-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  