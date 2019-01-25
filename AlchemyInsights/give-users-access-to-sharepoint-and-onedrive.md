---
title: Ge användare åtkomst till SharePoint och OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498032"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="d2f96-102">Ge användare åtkomst till SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="d2f96-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="d2f96-p101">Om en OneDrive eller SharePoint-webbplatsen inte är tillgänglig för flera användare som tidigare har haft åtkomst kan det finnas en tillfällig service-problem. [Kontrollera att tjänsten hälsa instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="d2f96-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="d2f96-p102">Om du vill att personer i organisationen för att kunna logga in och använda SharePoint och OneDrive, måste du lägga till konton för dem och kontrollera att de har en licens som ger dem tillgång till SharePoint och OneDrive. Det är det enklaste sättet att lägga till användare i Office 365 administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="d2f96-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="d2f96-107">Gå till [sidan aktiv användare i Office 365 administratörscenter](https://portal.office.com/adminportal/home#/users)och klicka sedan på **Lägg till en användare**.</span><span class="sxs-lookup"><span data-stu-id="d2f96-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="d2f96-108">Fyll i information om användaren och se till att **licenser**tilldelas en licens och **SharePoint Online** är markerad.</span><span class="sxs-lookup"><span data-stu-id="d2f96-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="d2f96-p103">Observera att om du tillåter extern delning i organisationen, användarna kan dela innehåll i SharePoint och OneDrive med personer utanför organisationen. Du behöver inte ge dessa licenser för externa användare. Du också behöver inte lägga till konton för dem, såvida inte dela är inställd på ”endast befintliga externa användare”. I så fall om personerna som inte finns med i organisationens katalog måste du lägga till dem som gästanvändare i Azure AD administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="d2f96-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

