---
title: Åtgärda problem med e-post levereras till e-postfunktioner gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752698"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="d090d-102">Åtgärda problem med e-post levereras till e-postfunktioner gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="d090d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="d090d-103">Om externa avsändare kan inte skicka meddelanden till din e-postfunktioner gemensamma mappar och avsändare visas fel: **kunde inte hittas (550 5.4.1)**, verifiera e-domänen för den gemensamma mappen konfigureras som en intern relay domän i stället för en auktoritär domän:</span><span class="sxs-lookup"><span data-stu-id="d090d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="d090d-104">Öppna [Exchange administratörscenter (UK)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="d090d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="d090d-105">Gå till **e-postflödet** \> **accepterade domäner**, markera accepterade domänen och klicka sedan på **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="d090d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="d090d-106">I egenskaperna för sidan som öppnas om typen domän är **auktoritära**, ändra värdet till **interna relay** och klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="d090d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="d090d-107">Om externa avsändare får fel **du inte har behörighet (550 5.7.13)**, kör du följande kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) Se behörigheter för anonyma användare i den delade mappen:</span><span class="sxs-lookup"><span data-stu-id="d090d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="d090d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="d090d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="d090d-109">Tillåt externa användare att skicka e-post till mappen genom att lägga till CreateItems access rätt till användaren Anonym.</span><span class="sxs-lookup"><span data-stu-id="d090d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="d090d-110">Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="d090d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
