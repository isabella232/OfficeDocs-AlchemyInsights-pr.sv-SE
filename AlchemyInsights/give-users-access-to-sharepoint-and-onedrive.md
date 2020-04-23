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
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Ge användarna åtkomst till SharePoint och OneDrive

> [!NOTE]
> Om en OneDrive- eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem. [Kontrollera instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth)
  
Om du vill att personer i organisationen ska kunna logga in och använda SharePoint och OneDrive måste du lägga till konton för dem och se till att de har en licens som ger dem åtkomst till SharePoint och OneDrive. Det enklaste sättet att lägga till användare finns i microsoft 365 admin center.
  
1. Gå till [sidan Aktiva användare i administrationscentret för Microsoft 365](https://portal.office.com/adminportal/home#/users)och klicka sedan på Lägg till en **användare**.
    
2. Fyll i informationen för användaren och se till att under **Produktlicenser**tilldelas en licens och **SharePoint Online** väljs. 
    
Observera att om du tillåter extern delning i organisationen kan användarna dela SharePoint- och OneDrive-innehåll med personer utanför organisationen. Du behöver inte ge dessa externa användare licenser. Du behöver inte heller lägga till konton för dem, såvida inte delning är inställd på "Endast befintliga externa användare". I så fall, om personerna inte finns i organisationens katalog, måste du lägga till dem som gästanvändare i Azure AD-administrationscentret.
  

