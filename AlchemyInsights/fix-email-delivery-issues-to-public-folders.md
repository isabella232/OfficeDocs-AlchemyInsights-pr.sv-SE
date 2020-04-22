---
title: Åtgärda problem med e-postleverans på e-postaktiverade gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716370"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="dd6e7-102">Åtgärda problem med e-postleverans på e-postaktiverade gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="dd6e7-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="dd6e7-103">Om externa avsändare inte kan skicka meddelanden till dina e-postaktiverade gemensamma mappar och avsändarna får **felmeddelandet: det gick inte att hitta (550 5.4.1)** kontrollerar du att e-postdomänen för den gemensamma mappen är konfigurerad som en intern relay-domän i stället för en auktoritär domän:</span><span class="sxs-lookup"><span data-stu-id="dd6e7-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="dd6e7-104">Öppna [Administrationscentret för Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="dd6e7-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="dd6e7-105">Gå till **Domäner för** **e-postflöde** \> Accepterade, välj den accepterade domänen och klicka sedan på **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="dd6e7-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="dd6e7-106">Om domäntypen är inställd på **Auktoritär**på egenskapssidan som öppnas ändrar du värdet till **Internt relä** och klickar sedan på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="dd6e7-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="dd6e7-107">Om externa avsändare får felet **som du inte har behörighet (550 5.7.13)** kör du följande kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) för att se behörigheterna för anonyma användare i den gemensamma mappen:</span><span class="sxs-lookup"><span data-stu-id="dd6e7-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="dd6e7-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="dd6e7-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="dd6e7-109">Om du vill att externa användare ska kunna skicka e-post till den här gemensamma mappen lägger du till åtkomsten till CreateItems till användaren Anonym.</span><span class="sxs-lookup"><span data-stu-id="dd6e7-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="dd6e7-110">Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="dd6e7-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
