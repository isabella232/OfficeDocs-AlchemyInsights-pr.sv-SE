---
title: Korrigera problem med e-postleverans till e-postaktiverade gemensamma mappar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677946"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="09139-102">Korrigera problem med e-postleverans till e-postaktiverade gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="09139-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="09139-103">Om externa avsändare inte kan skicka meddelanden till dina e-postaktiverade gemensamma mappar och avsändarna får felet: **kunde inte hittas (550 5.4.1)** kontrollerar du att e-postdomänen är konfigurerad som en intern Relay-domän i stället för en auktoritativ domän:</span><span class="sxs-lookup"><span data-stu-id="09139-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="09139-104">Öppna [administrations centret för Exchange (UK)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="09139-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="09139-105">Gå till **e-postflöden** \> **godkända domäner**, Välj den godkända domänen och klicka sedan på **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="09139-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="09139-106">Om domän typen är inställd på **auktoritär**på sidan egenskaper kan du ändra värdet till **intern relä** och klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="09139-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="09139-107">Om externa avsändare får felet att **du inte har behörighet (550 5.7.13)** kör du följande kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) för att se behörigheterna för anonyma användare i den gemensamma mappen:</span><span class="sxs-lookup"><span data-stu-id="09139-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="09139-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Till exempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="09139-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="09139-109">Om du vill tillåta externa användare att skicka e-post till den här gemensamma mappen lägger du till åtkomsten CreateItems till användaren anonym.</span><span class="sxs-lookup"><span data-stu-id="09139-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="09139-110">Till exempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="09139-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
