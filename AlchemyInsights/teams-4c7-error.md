---
title: Lag 4c7 fel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796408"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="2458f-102">4c7-fel i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2458f-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="2458f-103">Det här felet beror på att Microsoft Teams kräver formulärautentisering.</span><span class="sxs-lookup"><span data-stu-id="2458f-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="2458f-104">När du distribuerar Active Directory Federation Services (AD FS) är formulärautentisering inte aktiverat för intranätet som standard.</span><span class="sxs-lookup"><span data-stu-id="2458f-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="2458f-105">Om Windows-integrerad autentisering misslyckas uppmanas du att logga in med formulärautentisering.</span><span class="sxs-lookup"><span data-stu-id="2458f-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="2458f-106">Lös problemet genom att aktivera formulärautentisering med hjälp av snapin-modulen AD FS Microsoft Management Console (MMC) på den dator som har den lokala kopian av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2458f-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="2458f-107">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="2458f-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="2458f-108">I navigeringsfönstret bläddrar du till **autentiseringsprinciper**.</span><span class="sxs-lookup"><span data-stu-id="2458f-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="2458f-109">Välj **Redigera global primär autentisering**under **åtgärder** i informationsfönstret.</span><span class="sxs-lookup"><span data-stu-id="2458f-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="2458f-110">Välj **formulärautentisering**på fliken **intranät** .</span><span class="sxs-lookup"><span data-stu-id="2458f-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="2458f-111">Välj **OK** (eller **Verkställ**).</span><span class="sxs-lookup"><span data-stu-id="2458f-111">Select **OK** (or **Apply**).</span></span>