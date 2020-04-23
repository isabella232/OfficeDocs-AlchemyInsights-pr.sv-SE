---
title: Ge användarna åtkomst till SharePoint och OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721846"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="3cb1e-102">Ge användarna åtkomst till SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="3cb1e-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="3cb1e-103">Om en OneDrive- eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="3cb1e-104">Kontrollera instrumentpanelen för tjänstens hälsa</span><span class="sxs-lookup"><span data-stu-id="3cb1e-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="3cb1e-105">Om du vill att personer i organisationen ska kunna logga in och använda SharePoint och OneDrive måste du lägga till konton för dem och se till att de har en licens som ger dem åtkomst till SharePoint och OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="3cb1e-106">Det enklaste sättet att lägga till användare finns i microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="3cb1e-107">Gå till [sidan Aktiva användare i administrationscentret för Microsoft 365](https://portal.office.com/adminportal/home#/users)och klicka sedan på Lägg till en **användare**.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="3cb1e-108">Fyll i informationen för användaren och se till att under **Produktlicenser**tilldelas en licens och **SharePoint Online** väljs.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="3cb1e-109">Observera att om du tillåter extern delning i organisationen kan användarna dela SharePoint- och OneDrive-innehåll med personer utanför organisationen.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="3cb1e-110">Du behöver inte ge dessa externa användare licenser.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="3cb1e-111">Du behöver inte heller lägga till konton för dem, såvida inte delning är inställd på "Endast befintliga externa användare".</span><span class="sxs-lookup"><span data-stu-id="3cb1e-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="3cb1e-112">I så fall, om personerna inte finns i organisationens katalog, måste du lägga till dem som gästanvändare i Azure AD-administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="3cb1e-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

