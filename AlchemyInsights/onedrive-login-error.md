---
title: Fel i OneDrive-AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982547"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="381ba-102">Fel i OneDrive-AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="381ba-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="381ba-103">Om du får ett fel meddelande om att svars-URL: en som angetts i begäran inte matchar svaret "när du loggar in på OneDrive-appen, kan du kontrol lera följande:</span><span class="sxs-lookup"><span data-stu-id="381ba-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="381ba-104">Din OneDrive-version måste vara lika med eller större än version 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="381ba-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="381ba-105">Kontrol lera din version genom att klicka på den blå OneDrive-ikonen i meddelande fältet, Välj **hjälp & inställningar > inställningar > om**.</span><span class="sxs-lookup"><span data-stu-id="381ba-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="381ba-106">Nätverket kan blockera trafik till **g.live.com** och **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="381ba-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="381ba-107">Om den trafiken är blockerad kan OneDrive inte uppdatera sig själv.</span><span class="sxs-lookup"><span data-stu-id="381ba-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="381ba-108">Arbeta med nätverks administratören för att se till att du har åtkomst till dessa URL: er.</span><span class="sxs-lookup"><span data-stu-id="381ba-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="381ba-109">[Dessa slut punkter](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) bör kunna nås för kunder som använder Microsoft 365-abonnemang.</span><span class="sxs-lookup"><span data-stu-id="381ba-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="381ba-110">Om du behöver skaffa en aktuell version av OneDrive manuellt kan du gå till [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="381ba-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
