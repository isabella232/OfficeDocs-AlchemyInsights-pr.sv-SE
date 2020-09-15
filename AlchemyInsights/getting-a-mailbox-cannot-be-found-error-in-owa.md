---
title: 126 Det går inte att hitta ett fel meddelande i OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706768"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="dacf1-102">Det går inte att få ett brev låde fel i Outlook på webben?</span><span class="sxs-lookup"><span data-stu-id="dacf1-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="dacf1-103">Om du använder Outlook på webben och det **inte går att hitta en post låda för** felet har kontot som du använde för att ansluta till Outlook på webben ingen Exchange Online-licens och därför är inte post lådan kopplad till kontot.</span><span class="sxs-lookup"><span data-stu-id="dacf1-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="dacf1-104">Administratören kan tilldela en licens till ditt konto genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="dacf1-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="dacf1-105">Öppna [administrations centret för Microsoft 365](https://portal.office.com/adminportal/home#/homepage) och gå till **aktiva användare** under avsnittet **användare** och välj den användare som ska se felet.</span><span class="sxs-lookup"><span data-stu-id="dacf1-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="dacf1-106">Gå till avsnittet **licenser och program** på användar sidan som öppnas, Välj lämpligt **plats** värde och tilldela en licens som innehåller Exchange Online (expandera licensen för att se dess uppgifter).</span><span class="sxs-lookup"><span data-stu-id="dacf1-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="dacf1-107">När du är klar klickar du på **Spara ändringar**.</span><span class="sxs-lookup"><span data-stu-id="dacf1-107">When you're finished, click **Save changes**.</span></span>
