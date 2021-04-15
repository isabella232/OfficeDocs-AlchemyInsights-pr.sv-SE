---
title: Teams 4c7-fel
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786687"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="67797-102">4c7-fel i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="67797-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="67797-103">Det här felet inträffar eftersom Microsoft Teams kräver autentisering med formulär.</span><span class="sxs-lookup"><span data-stu-id="67797-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="67797-104">När du distribuerar AD FS (Active Directory Federation Services) aktiveras inte formulärautentisering för intranätet som standard.</span><span class="sxs-lookup"><span data-stu-id="67797-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="67797-105">Om Windows-integrerad autentisering inte fungerar uppmanas du att logga in med formsautentisering.</span><span class="sxs-lookup"><span data-stu-id="67797-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="67797-106">Lös problemet genom att aktivera formulärautentisering med hjälp av SNAPIN-modulen AD FS Microsoft Management Console (MMC) på datorn med den lokala kopian av Active Directory.</span><span class="sxs-lookup"><span data-stu-id="67797-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="67797-107">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="67797-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="67797-108">Bläddra till Autentiseringsprinciper i **navigeringsfönstret.**</span><span class="sxs-lookup"><span data-stu-id="67797-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="67797-109">Under **Åtgärder** i informationsfönstret väljer du **Redigera global primär autentisering**.</span><span class="sxs-lookup"><span data-stu-id="67797-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="67797-110">På fliken **Intranät** väljer du Autentisering **med formulär**.</span><span class="sxs-lookup"><span data-stu-id="67797-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="67797-111">Välj **OK** (eller **Använd**).</span><span class="sxs-lookup"><span data-stu-id="67797-111">Select **OK** (or **Apply**).</span></span>