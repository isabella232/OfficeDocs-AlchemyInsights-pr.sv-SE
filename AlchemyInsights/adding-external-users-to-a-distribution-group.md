---
title: Lägga till externa användare i en distributions grupp
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663531"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="1b92b-102">Lägga till externa användare i en distributions grupp</span><span class="sxs-lookup"><span data-stu-id="1b92b-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="1b92b-103">Att lägga till en extern kontakt i en distributions grupp är en process i två steg:</span><span class="sxs-lookup"><span data-stu-id="1b92b-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="1b92b-104">Skapa en e-postkontakt för den externa användaren:</span><span class="sxs-lookup"><span data-stu-id="1b92b-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="1b92b-105">Gå till sidan **användare**kontakter i administrations centret  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="1b92b-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="1b92b-106">Välj **Lägg till en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="1b92b-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="1b92b-107">Skriv informationen för kontakten och välj **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="1b92b-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="1b92b-108">Lägg till e-postkontakten till din DG:</span><span class="sxs-lookup"><span data-stu-id="1b92b-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="1b92b-109">Gå till sidan grupper i administrations centret **Groups**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="1b92b-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="1b92b-110">Leta reda på den DG som du vill lägga till den externa användaren i och välj den för att öppna dialog rutan Redigera.</span><span class="sxs-lookup"><span data-stu-id="1b92b-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="1b92b-111">På fliken **medlemmar** väljer du **Visa alla och hantera medlemmar**.</span><span class="sxs-lookup"><span data-stu-id="1b92b-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="1b92b-112">Välj **Lägg till medlemmar**.</span><span class="sxs-lookup"><span data-stu-id="1b92b-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="1b92b-113">Markera den e-postkontakt som du skapade i föregående steg och välj sedan **Spara**.</span><span class="sxs-lookup"><span data-stu-id="1b92b-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="1b92b-114">Om de externa användarna inte kan skicka e-post till DG eller inte ta emot e-post från den här proceduren, kan det bero på att DG är markerat för att endast tillåta e-post från interna användare.</span><span class="sxs-lookup"><span data-stu-id="1b92b-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="1b92b-115">Du kan kontrol lera denna konfiguration och åtgärda den enligt anvisningarna [här](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="1b92b-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="1b92b-116">**Obs!** De här instruktionerna gäller inte om gruppens typ är "Microsoft 365 Group" i stället för "distribution Group".</span><span class="sxs-lookup"><span data-stu-id="1b92b-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="1b92b-117">Om så är fallet kan du lägga till den externa användaren direkt i gruppen från Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b92b-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="1b92b-118">Detaljerad information om Microsoft 365-grupp gäster och anvisningar för att lägga till externa gäster finns i [den här artikeln](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="1b92b-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  