---
title: Teams 4c7-fel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700221"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="a01a4-102">4c7 fel i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a01a4-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="a01a4-103">Det här felet beror på att Microsoft Teams kräver formulärautentisering.</span><span class="sxs-lookup"><span data-stu-id="a01a4-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="a01a4-104">När du distribuerar AD FS (Active Directory Federation Services) är formulärautentisering inte aktiverat för intranätet som standard.</span><span class="sxs-lookup"><span data-stu-id="a01a4-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="a01a4-105">Om Windows-integrerad autentisering inte fungerar uppmanas du att logga in med formulärautentisering.</span><span class="sxs-lookup"><span data-stu-id="a01a4-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="a01a4-106">Lös problemet genom att aktivera formulärautentisering med snapin-modulen AD FS Microsoft Management Console (MMC) på den dator som har den lokala kopian av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a01a4-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="a01a4-107">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="a01a4-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="a01a4-108">Bläddra till **autentiseringsprinciper**i navigerings fönstret.</span><span class="sxs-lookup"><span data-stu-id="a01a4-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="a01a4-109">Välj **Redigera global primär verifikation**under **åtgärder** i informations fönstret.</span><span class="sxs-lookup"><span data-stu-id="a01a4-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="a01a4-110">Välj **formulärautentisering**på fliken **intranät** .</span><span class="sxs-lookup"><span data-stu-id="a01a4-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="a01a4-111">Välj **OK** (eller **Använd**).</span><span class="sxs-lookup"><span data-stu-id="a01a4-111">Select **OK** (or **Apply**).</span></span>